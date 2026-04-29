---
description: ''
layout: schema
name: Error
properties_list:
- description: The application name that generated this error. Every error message that is generated and returned by the gateway will have this field equal to Gateway.
  name: Source
  type: string
- description: A unique constant identifying the error case encountered during request processing.
  name: ReasonCode
  type: string
- description: Short description of the ReasonCode field.
  name: Description
  type: string
- description: Indicates whether this error will always be returned for this request, or retrying could change the outcome.
  name: Recoverable
  type: boolean
- description: (Optional) Where appropriate, indicates detailed information about data received and calculated during request processing, to help the customer with diagnosing errors.
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-automatic-billing-updater-error-schema.json
slug: mastercard-automatic-billing-updater-error
source_filename: mastercard-automatic-billing-updater-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"The application name that generated this error. Every error message that is generated and returned by the gateway will have this field equal to Gateway.\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A unique constant identifying the error case encountered during request processing.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the ReasonCode field.\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this error will always be returned for this request, or retrying could change the outcome.\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"(Optional) Where appropriate, indicates\
  \ detailed information about data received and calculated during request processing, to help the customer with diagnosing errors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-automatic-billing-updater-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
