---
description: Schema for a Nasdaq Data Link (formerly Quandl) time-series dataset record, including metadata and data rows.
layout: schema
name: Nasdaq Data Link Dataset
properties_list:
- description: Internal Nasdaq Data Link dataset identifier
  name: id
  type: integer
- description: Dataset code within its database (e.g., AAPL, GDP, CL1)
  name: dataset_code
  type: string
- description: Database code (e.g., WIKI, FRED, CHRIS, BCOM)
  name: database_code
  type: string
- description: Human-readable dataset name
  name: name
  type: string
- description: Detailed dataset description including source and coverage
  name: description
  type: string
- description: Timestamp when dataset was last refreshed with new data
  name: refreshed_at
  type: string
- description: Most recent date with available data
  name: newest_available_date
  type: string
- description: Oldest date with available data
  name: oldest_available_date
  type: string
- description: Ordered list of column names matching data row positions
  name: column_names
  type: array
- description: Native data frequency
  name: frequency
  type: string
- description: Dataset type
  name: type
  type: string
- description: True if access to this dataset requires a paid subscription
  name: premium
  type: boolean
- description: Data rows; each row is an array matching column_names order. First element is always a date string.
  name: data
  type: array
- description: Start of returned date range
  name: start_date
  type: string
- description: End of returned date range
  name: end_date
  type: string
provider_name: Quandl (Nasdaq Data Link)
provider_slug: quandl
schema_file: json-schema/nasdaq-data-link-dataset-schema.json
slug: nasdaq-data-link-dataset
source_filename: nasdaq-data-link-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/quandl/json-schema/nasdaq-data-link-dataset-schema.json\",\n  \"title\": \"Nasdaq Data Link Dataset\",\n  \"description\": \"Schema for a Nasdaq Data Link (formerly Quandl) time-series dataset record, including metadata and data rows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Nasdaq Data Link dataset identifier\"\n    },\n    \"dataset_code\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset code within its database (e.g., AAPL, GDP, CL1)\"\n    },\n    \"database_code\": {\n      \"type\": \"string\",\n      \"description\": \"Database code (e.g., WIKI, FRED, CHRIS, BCOM)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable dataset name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Detailed dataset description including source and coverage\"\n    },\n    \"refreshed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when dataset was last refreshed with new data\"\n    },\n    \"newest_available_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Most recent date with available data\"\n    },\n    \"oldest_available_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Oldest date with available data\"\n    },\n    \"column_names\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of column names matching data row positions\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"examples\": [\n        [\"Date\", \"Open\", \"High\", \"Low\", \"Close\", \"Volume\", \"Adj. Close\"],\n        [\"Date\", \"Value\"],\n        [\"Date\", \"Open\", \"High\", \"Low\", \"Settle\"\
  , \"Volume\", \"Open Interest\"]\n      ]\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"enum\": [\"annual\", \"quarterly\", \"monthly\", \"weekly\", \"daily\"],\n      \"description\": \"Native data frequency\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Time Series\"],\n      \"description\": \"Dataset type\"\n    },\n    \"premium\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if access to this dataset requires a paid subscription\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Data rows; each row is an array matching column_names order. First element is always a date string.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"number\" },\n            { \"type\": \"null\" }\n          ]\n        }\n      }\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n   \
  \   \"format\": \"date\",\n      \"description\": \"Start of returned date range\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End of returned date range\"\n    }\n  },\n  \"required\": [\"dataset_code\", \"database_code\", \"name\", \"column_names\", \"frequency\"],\n  \"examples\": [\n    {\n      \"id\": 9775687,\n      \"dataset_code\": \"AAPL\",\n      \"database_code\": \"WIKI\",\n      \"name\": \"Apple Inc. (AAPL) Prices, Dividends, Splits and Trading Volume\",\n      \"description\": \"End of day open, high, low, close and volume, dividends and splits, and split/dividend adjusted open, high, low close and volume for Apple Inc. (AAPL).\",\n      \"refreshed_at\": \"2018-03-27T21:46:11.849Z\",\n      \"newest_available_date\": \"2018-03-27\",\n      \"oldest_available_date\": \"1980-12-12\",\n      \"column_names\": [\"Date\", \"Open\", \"High\", \"Low\", \"Close\", \"Volume\", \"Ex-Dividend\", \"Split Ratio\"\
  , \"Adj. Open\", \"Adj. High\", \"Adj. Low\", \"Adj. Close\", \"Adj. Volume\"],\n      \"frequency\": \"daily\",\n      \"type\": \"Time Series\",\n      \"premium\": false,\n      \"data\": [\n        [\"2018-03-27\", 173.68, 175.15, 166.92, 168.34, 38962839.0, 0.0, 1.0, 173.68, 175.15, 166.92, 168.34, 38962839.0]\n      ],\n      \"start_date\": \"2018-03-27\",\n      \"end_date\": \"2018-03-27\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quandl/refs/heads/main/json-schema/nasdaq-data-link-dataset-schema.json
tags:
- Finance
- Market Data
- Economic Data
- Time Series
- Streaming
title: Nasdaq Data Link Dataset
---
