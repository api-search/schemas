---
description: ServiceErrorDetails schema from Adyen API
layout: schema
name: ServiceErrorDetails
properties_list:
- description: ''
  name: errorCode
  type: string
- description: ''
  name: errorType
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: pspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-service-error-details-schema.json
slug: checkout-service-error-details
source_filename: checkout-service-error-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-service-error-details-schema.json\",\n  \"title\": \"ServiceErrorDetails\",\n  \"description\": \"ServiceErrorDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\"\n    },\n    \"errorType\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-service-error-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ServiceErrorDetails
---
