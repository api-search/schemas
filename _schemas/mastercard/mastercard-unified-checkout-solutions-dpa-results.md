---
description: Status of uploaded dpas
layout: schema
name: DpaResults
properties_list:
- description: generated id for srci dpa
  name: srciDpaId
  type: string
- description: 'Status of the individual Digital Payment Application (DPA) item. Potential statuses include: * `SUCCESSFUL` - The DPA is eligible to process transactions. * `FAILED` - The DPA is NOT eligible to proce'
  name: status
  type: string
- description: Registered Legal Name of the Merchant
  name: dpaName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-dpa-results-schema.json
slug: mastercard-unified-checkout-solutions-dpa-results
source_filename: mastercard-unified-checkout-solutions-dpa-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DpaResults\",\n  \"type\": \"object\",\n  \"description\": \"Status of uploaded dpas\",\n  \"properties\": {\n    \"srciDpaId\": {\n      \"type\": \"string\",\n      \"description\": \"generated id for srci dpa\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the individual Digital Payment Application (DPA) item. Potential statuses include:\\n\\n* `SUCCESSFUL` - The DPA is eligible to process transactions.\\n* `FAILED` - The DPA is NOT eligible to process transactions. Please see the error object for more details.\\n\"\n    },\n    \"dpaName\": {\n      \"type\": \"string\",\n      \"description\": \"Registered Legal Name of the Merchant\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-dpa-results-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DpaResults
---
