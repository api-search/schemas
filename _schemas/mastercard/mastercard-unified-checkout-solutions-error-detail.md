---
description: Error associated with a failed Digital Payment Application (DPA) item action.
layout: schema
name: ErrorDetail
properties_list:
- description: Reason for receiving an error for the Digital Payment Application (DPA) item.
  name: reason
  type: string
- description: Indicates the source type of the Digital Payment Application (DPA) item error.
  name: sourceType
  type: string
- description: Additional details on the Digital Payment Application (DPA) item error.
  name: message
  type: string
- description: Indicates the field name for the cause of the Digital Payment Application (DPA) item error.
  name: source
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-error-detail-schema.json
slug: mastercard-unified-checkout-solutions-error-detail
source_filename: mastercard-unified-checkout-solutions-error-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\",\n  \"type\": \"object\",\n  \"description\": \"Error associated with a failed Digital Payment Application (DPA) item action.\",\n  \"properties\": {\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for receiving an error for the Digital Payment Application (DPA) item.\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the source type of the Digital Payment Application (DPA) item error.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details on the Digital Payment Application (DPA) item error.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the field name for the cause of the Digital Payment Application (DPA) item error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-error-detail-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ErrorDetail
---
