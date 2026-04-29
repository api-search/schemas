---
description: ''
layout: schema
name: Error
properties_list:
- description: The source of the problem. i.e where the error occurred
  name: Source
  type: string
- description: A code defining the error, as defined in documentation
  name: ReasonCode
  type: string
- description: A description for this specific occurrence of the above ReasonCode
  name: Description
  type: string
- description: Whether or not retrying this request could result in a successful response.
  name: Recoverable
  type: boolean
- description: More details of this specific error. This is an optional field and is sometimes used to give a more comprehensive description of the error that has occurred, when required.
  name: Details
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-error-schema.json
slug: mastercard-identity-insights-for-transactions-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the problem. i.e where the error occurred\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A code defining the error, as defined in documentation\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for this specific occurrence of the above ReasonCode\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether or not retrying this request could result in a successful response.\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"More details of this specific error. This is an optional field and is sometimes used to give a more comprehensive description of the error that has occurred, when required.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
