---
description: An Amazon Forecast ML predictor trained on a dataset group.
layout: schema
name: Predictor
properties_list:
- description: ARN of the predictor.
  name: PredictorArn
  type: string
- description: Name of the predictor.
  name: PredictorName
  type: string
- description: ARN of the algorithm used.
  name: AlgorithmArn
  type: string
- description: Number of time steps for the forecast.
  name: ForecastHorizon
  type: integer
- description: Quantiles to forecast (e.g., p10, p50, p90).
  name: ForecastTypes
  type: array
- description: Whether to auto-select the best algorithm.
  name: PerformAutoML
  type: boolean
- description: Whether to perform hyperparameter optimization.
  name: PerformHPO
  type: boolean
- description: Status of the predictor.
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
schema_file: json-schema/amazon-forecast-predictor-schema.json
slug: amazon-forecast-predictor
source_filename: amazon-forecast-predictor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-predictor-schema.json\",\n  \"title\": \"Predictor\",\n  \"description\": \"An Amazon Forecast ML predictor trained on a dataset group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PredictorArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the predictor.\"\n    },\n    \"PredictorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the predictor.\"\n    },\n    \"AlgorithmArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the algorithm used.\"\n    },\n    \"ForecastHorizon\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of time steps for the forecast.\"\n    },\n    \"ForecastTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"Quantiles to forecast (e.g., p10, p50, p90).\"\n    },\n    \"PerformAutoML\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to auto-select the best algorithm.\"\n    },\n    \"PerformHPO\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to perform hyperparameter optimization.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the predictor.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastModificationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"PredictorName\",\n    \"ForecastHorizon\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-predictor-schema.json
tags:
- Forecasting
- Machine Learning
- Predictive Analytics
- Time Series
title: Predictor
---
