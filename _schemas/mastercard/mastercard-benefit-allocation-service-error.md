---
description: ''
layout: schema
name: Error
properties_list:
- description: Information about where the error happened
  name: Source
  type: string
- description: An error code
  name: ReasonCode
  type: string
- description: A description of the error
  name: Description
  type: string
- description: Indicates if the request can be presented again for processing
  name: Recoverable
  type: boolean
- description: More details about the error
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-error-schema.json
slug: mastercard-benefit-allocation-service-error
source_filename: mastercard-benefit-allocation-service-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"Information about where the error happened\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"An error code\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the error\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the request can be presented again for processing\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"More details about the error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
