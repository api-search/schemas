---
description: Details of the error condition such as the source of the error, reason code for the error, if the error is recoverable, and details about the error
layout: schema
name: Error
properties_list:
- description: The application that generated this error
  name: Source
  type: string
- description: A unique constant identifying the error case encountered during transaction processing
  name: ReasonCode
  type: string
- description: Short description of the ReasonCode field
  name: Description
  type: string
- description: Indicates whether this error will always be returned for this request, or retrying could change the outcome
  name: Recoverable
  type: boolean
- description: Description of the issue
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-atm-locations-error-schema.json
slug: mastercard-atm-locations-error
source_filename: mastercard-atm-locations-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Details of the error condition such as the source of the error, reason code for the error, if the error is recoverable, and details about the error\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"The application that generated this error\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A unique constant identifying the error case encountered during transaction processing\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the ReasonCode field\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this error will always be returned for this request, or retrying could change the outcome\"\n    },\n    \"Details\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Description of the issue\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-atm-locations-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
