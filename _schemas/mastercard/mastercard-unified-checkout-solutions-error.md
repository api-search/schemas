---
description: 'An error object is associated with individual DPA failures in a given batch. Please note: In the event of a SUCCESSFUL response, this error object may be sent as NULL.'
layout: schema
name: Error
properties_list:
- description: HTTP status code associated with the Digital Payment Application (DPA) item error
  name: status
  type: integer
- description: Reason for receiving an error for the Digital Payment Application (DPA) item.
  name: reason
  type: string
- description: Additional details on the Digital Payment Application (DPA) item error.
  name: message
  type: string
- description: List of errors associated with a failed Digital Payment Application (DPA) item action.
  name: errordetail
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-error-schema.json
slug: mastercard-unified-checkout-solutions-error
source_filename: mastercard-unified-checkout-solutions-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"An error object is associated with individual DPA failures in a given batch.\\nPlease note: In the event of a SUCCESSFUL response, this error object may be sent as NULL.\\n\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code associated with the Digital Payment Application (DPA) item error\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for receiving an error for the Digital Payment Application (DPA) item.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details on the Digital Payment Application (DPA) item error.\"\n    },\n    \"errordetail\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors associated with a failed Digital Payment Application (DPA) item action.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-error-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Error
---
