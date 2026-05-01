---
description: ListUsageTotalsResponse schema
layout: schema
name: ListUsageTotalsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: totals
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-list-usage-totals-response-schema.json
slug: inspector-list-usage-totals-response
source_filename: inspector-list-usage-totals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-usage-totals-response-schema.json\",\n  \"title\": \"ListUsageTotalsResponse\",\n  \"description\": \"ListUsageTotalsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListUsageTotalsNextToken\"\n        },\n        {\n          \"description\": \"The pagination parameter to be used on the next list operation to retrieve more items.\"\n        }\n      ]\n    },\n    \"totals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageTotalList\"\n        },\n        {\n          \"description\": \"An object with details on the total usage for the requested account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-usage-totals-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ListUsageTotalsResponse
---
