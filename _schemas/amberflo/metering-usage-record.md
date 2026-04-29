---
description: A usage record grouped by dimension values
layout: schema
name: UsageRecord
properties_list:
- description: Group dimension values for this record
  name: groupInfo
  type: object
- description: Time-series usage data points
  name: records
  type: array
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/metering-usage-record-schema.json
slug: metering-usage-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-usage-record-schema.json\",\n  \"title\": \"UsageRecord\",\n  \"description\": \"A usage record grouped by dimension values\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupInfo\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Group dimension values for this record\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"Time-series usage data points\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"type\": \"number\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-usage-record-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: UsageRecord
---
