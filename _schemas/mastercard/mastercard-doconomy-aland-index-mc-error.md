---
description: Error object which contains details about error
layout: schema
name: MCError
properties_list:
- description: The application name that generated this error. Every error message that is generated and returned by the gateway will have this field equal to Gateway. Other possible values are Doconomy-Proxy and Do
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
- description: (Optional) Where appropriate, indicates detailed information about data received and calculated during request processing, to help the user with diagnosing errors.
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-doconomy-aland-index-mc-error-schema.json
slug: mastercard-doconomy-aland-index-mc-error
source_filename: mastercard-doconomy-aland-index-mc-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCError\",\n  \"type\": \"object\",\n  \"description\": \"Error object which contains details about error\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"The application name that generated this error. Every error message that is generated and returned by the gateway will have this field equal to Gateway. Other possible values are Doconomy-Proxy and Doconomy.\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A unique constant identifying the error case encountered during request processing.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the ReasonCode field.\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this error will always be returned for this request, or retrying could change the\
  \ outcome.\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"(Optional) Where appropriate, indicates detailed information about data received and calculated during request processing, to help the user with diagnosing errors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-doconomy-aland-index-mc-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MCError
---
