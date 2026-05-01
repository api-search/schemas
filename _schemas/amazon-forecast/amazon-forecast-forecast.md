---
description: An Amazon Forecast output generated from a trained predictor.
layout: schema
name: Forecast
properties_list:
- description: ARN of the forecast.
  name: ForecastArn
  type: string
- description: Name of the forecast.
  name: ForecastName
  type: string
- description: ARN of the predictor used.
  name: PredictorArn
  type: string
- description: Forecast quantiles generated.
  name: ForecastTypes
  type: array
- description: Status of the forecast.
  name: Status
  type: string
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: LastModificationTime
  type: string
provider_name: Amazon Forecast
provider_slug: amazon-forecast
schema_file: json-schema/amazon-forecast-forecast-schema.json
slug: amazon-forecast-forecast
source_filename: amazon-forecast-forecast-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-forecast-schema.json\",\n  \"title\": \"Forecast\",\n  \"description\": \"An Amazon Forecast output generated from a trained predictor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ForecastArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the forecast.\"\n    },\n    \"ForecastName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the forecast.\"\n    },\n    \"PredictorArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the predictor used.\"\n    },\n    \"ForecastTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Forecast quantiles generated.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the forecast.\"\
  \n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastModificationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"ForecastName\",\n    \"PredictorArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-forecast-schema.json
tags:
- Forecasting
- Machine Learning
- Predictive Analytics
- Time Series
title: Forecast
---
