---
description: A single error.
layout: schema
name: Error
properties_list:
- description: Source of the error.
  name: Source
  type: string
- description: Error Code
  name: ReasonCode
  type: string
- description: Error Description.
  name: Description
  type: string
- description: Boolean value to specify if error is recoverable or not.
  name: Recoverable
  type: boolean
- description: Optional details of the error.
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-error-schema.json
slug: mastercard-debtor-service-provider-resources-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"A single error.\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the error.\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"Error Code\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Error Description.\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value to specify if error is recoverable or not.\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"Optional details of the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
