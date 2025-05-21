# sample-data
Pavan Kumar Kasani 
EXECUTE FUNCTION
TD_Plot
(
    SERIES_SPEC
    (
        TABLE_NAME(DEMO_AirPassengers.airpassengers),
        ROW_AXIS(TIMECODE("Date")),
        SERIES_ID(seriesID),
        PAYLOAD (FIELDS("Passengers"),CONTENT(REAL))
    ),
    FUNC_PARAMS
    (
        PLOTS[(
            TYPE('line'),
            LEGEND('upper left'),
            TITLE('Number of Passengers Traveling Monthly')
        )],
        IMAGE('png')
    )
);
