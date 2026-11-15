# FIT5202 — Big Data Processing: Spark & Kafka

> **Note:** this unit's results have not been released yet — keep this repo
> **private** until grades are out, then feel free to make it public.

PySpark and Kafka coursework analysing Melbourne parking, traffic, and sensor data:
batch processing and optimisation on large CSV/Parquet datasets, then a real-time
Kafka streaming pipeline (producer → Spark Structured Streaming → consumer).

## Contents

### `assignment1-spark-optimisation/`
*"Analysing Parking & Congestion Patterns in Melbourne"* — loading, cleaning and
validating large parking/traffic sensor datasets in PySpark (schema enforcement,
missing-value handling, timestamp parsing, duration calculation, data-quality
reporting), then partitioning and query optimisation with before/after evidence
from the Spark UI (jobs, stages, DAGs, shuffle read/write) in `screenshot/`.

### `assignment2a-batch-processing/`
Follow-up batch analysis on the same domain (parking sensors, traffic counts,
sites), building on the cleaned/partitioned data from Assignment 1.

### `assignment2b-kafka-streaming/`
Real-time streaming pipeline: a Kafka **producer** publishing live traffic/parking
events, a **Spark Structured Streaming** job consuming and processing the stream,
and a **consumer** reading the processed output.

## Tech stack

PySpark (DataFrames, Spark SQL, Structured Streaming), Apache Kafka, Jupyter.

## Note on data

The raw datasets (multi-GB CSVs of Melbourne parking/traffic sensor data, provided
by the unit) are not included here — only the notebooks, my written analysis, and
the Spark UI evidence.
