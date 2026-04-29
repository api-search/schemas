---
description: Request body for creating a meter definition
layout: schema
name: MeterDefinitionRequest
properties_list:
- description: Unique API name for the meter
  name: meterApiName
  type: string
- description: Human-readable display name
  name: displayName
  type: string
- description: Aggregation type for the meter
  name: type
  type: string
- description: Dimension names for this meter
  name: dimensions
  type: array
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/metering-meter-definition-request-schema.json
slug: metering-meter-definition-request
source_filename: metering-meter-definition-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-meter-definition-request-schema.json\",\n  \"title\": \"MeterDefinitionRequest\",\n  \"description\": \"Request body for creating a meter definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meterApiName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique API name for the meter\",\n      \"example\": \"api-calls\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name\",\n      \"example\": \"API Calls\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Aggregation type for the meter\",\n      \"enum\": [\n        \"SUM_OF_ALL_USAGE\",\n        \"MAX_IN_PERIOD\",\n        \"UNIQUE_CUSTOMERS_COUNT\"\n      ],\n      \"example\": \"SUM_OF_ALL_USAGE\"\n    },\n    \"dimensions\": {\n  \
  \    \"type\": \"array\",\n      \"description\": \"Dimension names for this meter\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"meterApiName\",\n    \"displayName\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-meter-definition-request-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: MeterDefinitionRequest
---
