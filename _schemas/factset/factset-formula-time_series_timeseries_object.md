---
description: The `result` attribute in the Time-Series Non-Flattened Response Object will be a TIMESERIES object. A TIMESERIES object has a values attribute and a dates attribute that contain arrays of equal length so that the values and dates can be align to form a time series.
layout: schema
name: time_series_timeseries_object
properties_list:
- description: Representing the data returned from the requested FQL formula for the requestId
  name: values
  type: array
- description: Representing the dates corresponding the requested FQL formula for the requestId
  name: dates
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-formula-time_series_timeseries_object-schema.json
slug: factset-formula-time_series_timeseries_object
source_filename: factset-formula-time_series_timeseries_object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"time_series_timeseries_object\",\n  \"type\": \"object\",\n  \"description\": \"The `result` attribute in the Time-Series Non-Flattened Response Object will be a TIMESERIES object. A TIMESERIES object has a values attribute and a dates attribute that contain arrays of equal length so that the values and dates can be align to form a time series.\",\n  \"properties\": {\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"Representing the data returned from the requested FQL formula for the requestId\"\n    },\n    \"dates\": {\n      \"type\": \"array\",\n      \"description\": \"Representing the dates corresponding the requested FQL formula for the requestId\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-formula-time_series_timeseries_object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: time_series_timeseries_object
---
