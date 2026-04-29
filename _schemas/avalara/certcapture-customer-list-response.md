---
description: CustomerListResponse schema from Avalara API
layout: schema
name: CustomerListResponse
properties_list:
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/certcapture-customer-list-response-schema.json
slug: certcapture-customer-list-response
source_filename: certcapture-customer-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-customer-list-response-schema.json\",\n  \"title\": \"CustomerListResponse\",\n  \"description\": \"CustomerListResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CertCaptureCustomer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/certcapture-customer-list-response-schema.json
tags:
- Taxes
title: CustomerListResponse
---
