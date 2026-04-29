---
description: DisputeServiceResult schema from Adyen API
layout: schema
name: DisputeServiceResult
properties_list:
- description: The general error message.
  name: errorMessage
  type: string
- description: Indicates whether the request succeeded.
  name: success
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-dispute-service-result-schema.json
slug: disputes-dispute-service-result
source_filename: disputes-dispute-service-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-dispute-service-result-schema.json\",\n  \"title\": \"DisputeServiceResult\",\n  \"description\": \"DisputeServiceResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorMessage\": {\n      \"description\": \"The general error message.\",\n      \"type\": \"string\"\n    },\n    \"success\": {\n      \"description\": \"Indicates whether the request succeeded.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"success\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-dispute-service-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisputeServiceResult
---
