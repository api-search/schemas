---
description: Schema for CRAN package download statistics from the METACRAN CranLogs API
layout: schema
name: CRAN Package Download Statistics
properties_list:
- description: R package name
  name: package
  type: string
- description: Start date of the download period
  name: start
  type: string
- description: End date of the download period
  name: end
  type: string
- description: ''
  name: downloads
  type: object
provider_name: R
provider_slug: r
schema_file: json-schema/r-download-stats-schema.json
slug: r-download-stats
source_filename: r-download-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/json-schema/r-download-stats-schema.json\",\n  \"title\": \"CRAN Package Download Statistics\",\n  \"description\": \"Schema for CRAN package download statistics from the METACRAN CranLogs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"package\": {\n      \"type\": \"string\",\n      \"description\": \"R package name\",\n      \"example\": \"ggplot2\"\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the download period\",\n      \"example\": \"2024-01-01\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of the download period\",\n      \"example\": \"2024-01-07\"\n    },\n    \"downloads\": {\n      \"oneOf\": [\n        {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Total download count for the period\",\n          \"example\": 142835\n        },\n        {\n          \"type\": \"array\",\n          \"description\": \"Daily breakdown of download counts\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"day\": {\n                \"type\": \"string\",\n                \"format\": \"date\",\n                \"description\": \"Date of the download count\"\n              },\n              \"downloads\": {\n                \"type\": \"integer\",\n                \"description\": \"Downloads on that day\"\n              }\n            },\n            \"required\": [\"day\", \"downloads\"]\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\"package\", \"start\", \"end\", \"downloads\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/json-schema/r-download-stats-schema.json
tags:
- R
- Statistics
- Data Science
- Open Source
- Programming Language
title: CRAN Package Download Statistics
---
