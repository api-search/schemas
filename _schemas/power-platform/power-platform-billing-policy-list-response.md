---
description: Response containing a list of billing policies.
layout: schema
name: BillingPolicyListResponse
properties_list:
- description: Array of billing policy resources.
  name: value
  type: array
- description: URL to retrieve the next page of results.
  name: '@odata.nextLink'
  type: '[''string'', ''null'']'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-billing-policy-list-response-schema.json
slug: power-platform-billing-policy-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BillingPolicyListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response containing a list of billing policies.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of billing policy resources.\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"URL to retrieve the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-billing-policy-list-response-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: BillingPolicyListResponse
---
