# azure-kusto-analytics-lib Repository

1. **KqlMagic**

    1. [Getting Started with KqlMagic](./KqlMagic/Getting-Started-With-KqlMagic-on-ADX.ipynb)

1. **Labs**

    1. [Custom Time Series Forecasting](./Lab/Custom-Time-Series-Forcasting/Time-Series-Forcast-Walkthrough.csl)<sup>[1](#footnotes)</sup> - build and tailor a time series forecasting model from lower level functions. See task [readme](./Lab/Custom-Time-Series-Forcasting/Time-Series-Forcast-Readme.docx) file
    1. [Classification](./Lab/Classifier) - [Build a classifier in Python](./Lab/Classifier/Prediction-of-Room-Occupancy-from-Kusto-Table-with-Kqlmagic.ipynb), [score](./Lab/Classifier/Classifier-Scoring.csl)<sup>[1](#footnotes)</sup> in ADX. See task [readme](./Lab/Classifier/Classifier-Readme.docx) file

1. **Machine Learning**

    * Functions

        1. [classify_sf()](./ML/functions/classify.csl)<sup>[1](#footnotes)</sup> - Classify (aka score) samples by a pre-trained model stored in models table
        1. [kmeans_sf()](./ML/functions/kmeans.csl)<sup>[1](#footnotes)</sup> - K-Means clustering

    * Queries

        1. [Clustering Plugins Tutorial](./ML/queries/Clustering-Plugins-Tutorial.csl) - Walkthrough of the clustering plugins for diagnosis & RCA
        1. [Python Plugin Tutorial](./ML/queries/Python-Plugin-Tutorial.csl)<sup>[1](#footnotes)</sup> - Walkthrough and demos of extending Kusto with inline Python

    * Notebooks

        1. [Training a classifier](./ML/notebooks/Prediction-of-Room-Occupancy-from-Kusto-Table-with-Kqlmagic.ipynb) - Demo of building and training a classifier for prediction of room occupancy in Jupyter using KqlMagic. Scoring is done using the Python plugin (see the [previous tutorial](./ML/queries/Python-Plugin-Tutorial.csl))
        
1. **Time Series Analysis**

    * Functions

        1. [blackman_filter_sf()](./Series/functions/blackman_filter.csl) - Create a Blackman window low pass filter of specific width
        1. [series_fit_poly_sf()](./Series/functions/series_fit_poly.csl)<sup>[1](#footnotes)</sup> - Fit a polynomial of a specified degree to a series
        1. [series_fit_sine_sf()](./Series/functions/series_fit_sine.csl)<sup>[1](#footnotes)</sup> - Fit a sine wave to a series
        1. [series_moving_avg_sf()](./Series/functions/series_moving_avg.csl) - Moving average of specific width
        1. [series_partial_sf()](./Series/functions/series_partial.csl) - Test for series with empty bins
        1. [series_rolling_sf()](./Series/functions/series_rolling.csl)<sup>[1](#footnotes)</sup> - Rolling window functions on a series
        1. [series_segment_sf()](./Series/functions/series_segment.csl) - Sequental numbering of non zero segments of a boolean series
        1. [series_summarize_sf()](./Series/functions/series_summarize.csl)<sup>[1](#footnotes)</sup> - Aggregation functions on a series
    * Queries

        1. [Time Series Analysis Tutorial](./Series/queries/Time-Series-Analysis-Tutorial.csl) - Walkthrough of typical series functions from each category

1. **Utils**

    * Functions
        1. [get_df_schema_sf()](./Utils/functions/get_df_schema.csl)<sup>[1](#footnotes)</sup> - Returns the schema of df (the DataFrame of the input table)
        1. [get_modules_version_sf()](./Utils/functions/get_modules_version.csl)<sup>[1](#footnotes)</sup> - Returns version information for the Python engine and the specified packages



<f name="footnotes">

**Notes:**

<sup>1</sup> Implementation using inline Python plugin
</f>