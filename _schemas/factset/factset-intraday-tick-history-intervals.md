---
description: ''
layout: schema
name: intervals
properties_list:
- description: Every Tick. Max days requested = 1
  name: '0'
  type: string
- description: 1 Second. Max days requested = 1
  name: 1S
  type: string
- description: 5 Seconds. Max days requested = 1
  name: 5S
  type: string
- description: 10 Seconds. Max days requested = 1
  name: 10S
  type: string
- description: 15 Seconds. Max days requested = 1
  name: 15S
  type: string
- description: 30 Seconds. Max days requested = 15
  name: 30S
  type: string
- description: 1 Minute. Max days requested = 30
  name: 1M
  type: string
- description: 2 Minutes. Max days requested = 60
  name: 2M
  type: string
- description: 5 Minutes. Max days requested = 60
  name: 5M
  type: string
- description: 10 Minutes. Max days requested = 60
  name: 10M
  type: string
- description: 15 Minutes. Max days requested = 60
  name: 15M
  type: string
- description: 30 Minutes. Max days requested = 60
  name: 30M
  type: string
- description: 1 Hour. Max days requested = 60
  name: 1H
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-intraday-tick-history-intervals-schema.json
slug: factset-intraday-tick-history-intervals
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"intervals\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"0\": {\n      \"type\": \"string\",\n      \"description\": \"Every Tick. Max days requested = 1\"\n    },\n    \"1S\": {\n      \"type\": \"string\",\n      \"description\": \"1 Second. Max days requested = 1\"\n    },\n    \"5S\": {\n      \"type\": \"string\",\n      \"description\": \"5 Seconds. Max days requested = 1\"\n    },\n    \"10S\": {\n      \"type\": \"string\",\n      \"description\": \"10 Seconds. Max days requested = 1\"\n    },\n    \"15S\": {\n      \"type\": \"string\",\n      \"description\": \"15 Seconds. Max days requested = 1\"\n    },\n    \"30S\": {\n      \"type\": \"string\",\n      \"description\": \"30 Seconds. Max days requested = 15\"\n    },\n    \"1M\": {\n      \"type\": \"string\",\n      \"description\": \"1 Minute. Max days requested = 30\"\n    },\n    \"2M\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"2 Minutes. Max days requested = 60\"\n    },\n    \"5M\": {\n      \"type\": \"string\",\n      \"description\": \"5 Minutes. Max days requested = 60\"\n    },\n    \"10M\": {\n      \"type\": \"string\",\n      \"description\": \"10 Minutes. Max days requested = 60\"\n    },\n    \"15M\": {\n      \"type\": \"string\",\n      \"description\": \"15 Minutes. Max days requested = 60\"\n    },\n    \"30M\": {\n      \"type\": \"string\",\n      \"description\": \"30 Minutes. Max days requested = 60\"\n    },\n    \"1H\": {\n      \"type\": \"string\",\n      \"description\": \"1 Hour. Max days requested = 60\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-intraday-tick-history-intervals-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: intervals
---
