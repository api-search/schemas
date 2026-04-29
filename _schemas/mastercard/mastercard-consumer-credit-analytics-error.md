---
description: ''
layout: schema
name: Error
properties_list:
- description: The name of the application that generated this error.
  name: Source
  type: string
- description: A unique constant identifying the error case encountered while processing the API request.
  name: ReasonCode
  type: string
- description: A short description of the ReasonCode field.
  name: Description
  type: string
- description: 'Indicates whether this error will always be returned for this request, or retrying could change the outcome. For example, if the request contains an invalid signature, retrying will never result in a '
  name: Recoverable
  type: boolean
- description: Where appropriate, indicates detailed information about data received and calculated during request processing, to help the user with diagnosing errors.
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-consumer-credit-analytics-error-schema.json
slug: mastercard-consumer-credit-analytics-error
source_filename: mastercard-consumer-credit-analytics-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application that generated this error.\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A unique constant identifying the error case encountered while processing the API request.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the ReasonCode field.\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this error will always be returned for this request, or retrying could change the outcome. For example, if the request contains an invalid signature, retrying will never result in a success. However, if the error is related to some unexpected timeout with the service, retrying the call could result\
  \ in a successful response.\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"Where appropriate, indicates detailed information about data received and calculated during request processing, to help the user with diagnosing errors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-consumer-credit-analytics-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
