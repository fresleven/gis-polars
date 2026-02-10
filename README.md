# gis-polars
A practical performance comparison between Polars and Pandas using real-world NYC taxi trip data.

## Overview

This benchmark demonstrates Polars' speed advantages over Pandas on large-scale geospatial data operations. Using NYC's publicly available taxi trip records (30M+ rows), we show **2-10x performance improvements** across common data analysis tasks including groupby operations, aggregations, and sorting. Performance gains come from Polars' parallel execution engine, lazy evaluation, and optimized memory management.

## Dataset

We use NYC Taxi & Limousine Commission trip record data:
- **Source**: [NYC TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- **Size**: 30M+ rows (multiple months combined)
- **Format**: Parquet files
- **Fields**: Pickup/dropoff locations, timestamps, distances, fares, passenger counts

## Why Polars?

- **Parallel Processing**: Automatic multi-threading
- **Lazy Evaluation**: Query optimization before execution
- **Memory Efficient**: Arrow-based columnar format
- **Expressive API**: Similar to Pandas with performance benefits
