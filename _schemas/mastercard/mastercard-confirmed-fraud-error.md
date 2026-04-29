---
description: ''
layout: schema
name: Error
properties_list:
- description: The application or component that generated this error.
  name: Source
  type: string
- description: Reason code is a unique constant identifying the error case encountered during request processing.
  name: ReasonCode
  type: string
- description: Human-readable short description of the reasonCode
  name: Description
  type: string
- description: Optional detailed description provides information about data received and calculated during request processing. This helps the user to diagnose errors.
  name: Details
  type: string
- description: Recoverable flag indicates whether this error is always returned for this request, or retrying could change the outcome. For example, 'true' or 'false'.
  name: Recoverable
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-confirmed-fraud-error-schema.json
slug: mastercard-confirmed-fraud-error
source_filename: mastercard-confirmed-fraud-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"The application or component that generated this error.\"\n    },\n    \"ReasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"Reason code is a unique constant identifying the error case encountered during request processing.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable short description of the reasonCode\"\n    },\n    \"Details\": {\n      \"type\": \"string\",\n      \"description\": \"Optional detailed description provides information about data received and calculated during request processing.  This helps the user to diagnose errors.\"\n    },\n    \"Recoverable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Recoverable flag indicates whether this error is always returned\
  \ for this request, or retrying could change the outcome.  For example, 'true' or 'false'.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-confirmed-fraud-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
