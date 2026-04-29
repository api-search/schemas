---
description: Standard CryptoQuant time-series API response envelope.
layout: schema
name: CryptoQuantTimeSeriesResponse
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: result
  type: object
provider_name: CryptoQuant
provider_slug: cryptoquant
schema_file: json-schema/cryptoquant-timeseries-schema.json
slug: cryptoquant-timeseries
source_filename: cryptoquant-timeseries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/json-schema/cryptoquant-timeseries-schema.json\",\n  \"title\": \"CryptoQuantTimeSeriesResponse\",\n  \"description\": \"Standard CryptoQuant time-series API response envelope.\",\n  \"type\": \"object\",\n  \"required\": [\"status\", \"result\"],\n  \"properties\": {\n    \"status\": {\n      \"type\": \"object\",\n      \"required\": [\"code\"],\n      \"properties\": {\n        \"code\": {\"type\": \"integer\"},\n        \"message\": {\"type\": \"string\"}\n      }\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"required\": [\"window\", \"data\"],\n      \"properties\": {\n        \"window\": {\"type\": \"string\", \"enum\": [\"min\", \"hour\", \"day\", \"block\"]},\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\"\
  : [\"date\"],\n            \"properties\": {\n              \"date\": {\"type\": \"string\", \"format\": \"date-time\"},\n              \"value\": {\"type\": \"number\"},\n              \"open\": {\"type\": \"number\"},\n              \"high\": {\"type\": \"number\"},\n              \"low\": {\"type\": \"number\"},\n              \"close\": {\"type\": \"number\"},\n              \"volume\": {\"type\": \"number\"}\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/json-schema/cryptoquant-timeseries-schema.json
tags:
- Blockchain
- Cryptocurrency
- On-Chain Analytics
- Market Data
- Derivatives
title: CryptoQuantTimeSeriesResponse
---
