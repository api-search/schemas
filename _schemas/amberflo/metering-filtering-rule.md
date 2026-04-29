---
description: A rule for filtering meter events before ingestion
layout: schema
name: FilteringRule
properties_list:
- description: The meter API name this rule applies to
  name: meterApiName
  type: string
- description: Unique identifier for this filtering rule
  name: ruleId
  type: string
- description: The dimension to filter on
  name: dimensionName
  type: string
- description: Values to include or exclude
  name: dimensionValues
  type: array
- description: Whether to include or exclude matching events
  name: action
  type: string
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/metering-filtering-rule-schema.json
slug: metering-filtering-rule
source_filename: metering-filtering-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-filtering-rule-schema.json\",\n  \"title\": \"FilteringRule\",\n  \"description\": \"A rule for filtering meter events before ingestion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meterApiName\": {\n      \"type\": \"string\",\n      \"description\": \"The meter API name this rule applies to\",\n      \"example\": \"api-calls\"\n    },\n    \"ruleId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this filtering rule\",\n      \"example\": \"rule-a1b2c3\"\n    },\n    \"dimensionName\": {\n      \"type\": \"string\",\n      \"description\": \"The dimension to filter on\",\n      \"example\": \"region\"\n    },\n    \"dimensionValues\": {\n      \"type\": \"array\",\n      \"description\": \"Values to include or exclude\",\n      \"items\": {\n        \"type\"\
  : \"string\"\n      },\n      \"example\": [\n        \"us-east-1\",\n        \"eu-west-1\"\n      ]\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to include or exclude matching events\",\n      \"enum\": [\n        \"INCLUDE\",\n        \"EXCLUDE\"\n      ],\n      \"example\": \"INCLUDE\"\n    }\n  },\n  \"required\": [\n    \"meterApiName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-filtering-rule-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: FilteringRule
---
