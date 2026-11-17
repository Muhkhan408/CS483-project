Data Preparation

We created a common Databricks workspace and uploaded our data to a Unity Catalog Volume:

/Volumes/workspace/default/farewise_data/

The taxi datasets are in taxi/, weather datasets in weather/, and the GeoJSON dataset in zones/. There are also processed/ and processed_final/ directories for saving the taxi-weather dataset.

What we've done so far:

Uploaded the complete taxi CSV, weather CSV, and taxi zones GeoJSON.
Loaded all three formats with PySpark and inspected their structures.
Inspected the number of records, missing values, and weird taxi values.
Converting the taxi features into numeric values and creating pickup timestamps.
Matched taxi trips with weather trips by pickup hours.
Creating the clean taxi-weather dataset and storing it in Parquet.
Reading the GeoJSON file, extracting its features, and counting 263 zones.
