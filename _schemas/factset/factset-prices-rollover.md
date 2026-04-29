---
description: ''
layout: schema
name: rollover
properties_list:
- description: Time of last zero date rollover for the Americas. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.
  name: americasRollTime
  type: string
- description: Current relative zero date for the Americas. Date is expressed in Eastern Time and expressed as YYYY-MM-DD.
  name: americasZeroDate
  type: string
- description: Time of last zero date rollover for Asia/Pacific. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.
  name: asiapacificRollTime
  type: string
- description: Current relative zero date for Asia/Pacific. This is in Eastern Time Zone
  name: asiapacificZeroDate
  type: string
- description: Time of last zero date rollover for Europe. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.
  name: europeRollTime
  type: string
- description: Current relative zero date for Europe. This is in Eastern Time Zone
  name: europeZeroDate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-rollover-schema.json
slug: factset-prices-rollover
source_filename: factset-prices-rollover-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"rollover\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"americasRollTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time of last zero date rollover for the Americas. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.\"\n    },\n    \"americasZeroDate\": {\n      \"type\": \"string\",\n      \"description\": \"Current relative zero date for the Americas. Date is expressed in Eastern Time and expressed as YYYY-MM-DD.\"\n    },\n    \"asiapacificRollTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time of last zero date rollover for Asia/Pacific. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.\"\n    },\n    \"asiapacificZeroDate\": {\n      \"type\": \"string\",\n      \"description\": \"Current relative zero date for Asia/Pacific.\
  \ This is in Eastern Time Zone\"\n    },\n    \"europeRollTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time of last zero date rollover for Europe. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.\"\n    },\n    \"europeZeroDate\": {\n      \"type\": \"string\",\n      \"description\": \"Current relative zero date for Europe. This is in Eastern Time Zone\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-rollover-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: rollover
---
