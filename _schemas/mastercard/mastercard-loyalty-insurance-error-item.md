---
description: ''
layout: schema
name: ErrorItem
properties_list:
- description: Source of the error.
  name: Source
  type: string
- description: Short description of the ReasonCode field.
  name: Description
  type: string
- description: A unique constant identifying the error case encountered during API request processing.
  name: ReasonCode
  type: string
- description: Indicates whether this error will always be returned for this request, or retrying could change the outcome.
  name: Recoverable
  type: boolean
- description: Where appropriate, indicates detailed information about data received.
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-loyalty-insurance-error-item-schema.json
slug: mastercard-loyalty-insurance-error-item
source_filename: mastercard-loyalty-insurance-error-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the error.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the ReasonCode field.\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A unique constant identifying the error case encountered during API request processing.\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this error will always be returned for this request, or retrying could change the outcome.\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"Where appropriate, indicates detailed information about data received.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-loyalty-insurance-error-item-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ErrorItem
---
