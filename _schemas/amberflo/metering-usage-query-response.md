---
description: Response from a usage data query
layout: schema
name: UsageQueryResponse
properties_list:
- description: Map of meter API name to usage records
  name: clientMeters
  type: object
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/metering-usage-query-response-schema.json
slug: metering-usage-query-response
source_filename: metering-usage-query-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-usage-query-response-schema.json\",\n  \"title\": \"UsageQueryResponse\",\n  \"description\": \"Response from a usage data query\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientMeters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"$ref\": \"#/components/schemas/UsageRecord\"\n        }\n      },\n      \"description\": \"Map of meter API name to usage records\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-usage-query-response-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: UsageQueryResponse
---
