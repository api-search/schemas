---
description: Resource with responseCode and details
layout: schema
name: BulkOperationResource
properties_list:
- description: List of error objects
  name: errors
  type: array
- description: The status of resource - PENDING, PASS, FAILED
  name: status
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-bulk-operation-resource-schema.json
slug: mastercard-ethoca-merchant-self-services-bulk-operation-resource
source_filename: mastercard-ethoca-merchant-self-services-bulk-operation-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BulkOperationResource\",\n  \"type\": \"object\",\n  \"description\": \"Resource with responseCode and details\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of error objects\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of resource - PENDING, PASS, FAILED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-bulk-operation-resource-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BulkOperationResource
---
