---
description: Error object
layout: schema
name: Error
properties_list:
- description: Source of the error
  name: Source
  type: string
- description: A unique constant identifying the error
  name: ReasonCode
  type: string
- description: Short description of the error
  name: Description
  type: string
- description: Indicates whether this error will always be returned for this request, or retrying could change the outcome
  name: Recoverable
  type: boolean
- description: Optional detailed description of the issue
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-error-schema.json
slug: mastercard-ethoca-merchant-self-services-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Error object\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the error\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A unique constant identifying the error\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the error\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this error will always be returned for this request, or retrying could change the outcome\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"Optional detailed description of the issue\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
