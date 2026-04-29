---
description: Object for individual Digital Payment Application (DPA) item status data.
layout: schema
name: DpaResults
properties_list:
- description: 'The registered identifier for the Digital Payment Application (DPA) accessing the service. Conditional: Required if you are a Merchant directly integrating with Mastercard Checkout Solutions (MCS) API'
  name: srcDpaId
  type: string
- description: 'Status of the individual Digital Payment Application (DPA) item. Potential statuses include: * SUCCESSFUL - The DPA is eligible to process transactions. * FAILED - The DPA is NOT eligible to process t'
  name: status
  type: string
- description: Legal name of Merchant (which may differ from dpaPresentationName).
  name: dpaName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-dpa-results-schema.json
slug: mastercard-checkout-solutions-dpa-results
source_filename: mastercard-checkout-solutions-dpa-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DpaResults\",\n  \"type\": \"object\",\n  \"description\": \"Object for individual Digital Payment Application (DPA) item status data.\",\n  \"properties\": {\n    \"srcDpaId\": {\n      \"type\": \"string\",\n      \"description\": \"The registered identifier for the Digital Payment Application (DPA) accessing the service.\\n\\nConditional: Required if you are a Merchant directly integrating with Mastercard Checkout Solutions (MCS) APIs, a Payment Service Provider (PSP) integrating On-Behalf-Of (OBO) a Merchant, a Payment Facilitator, or if you are enrolling in the Secure Card on File (SCOF) QR program.\\n\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the individual Digital Payment Application (DPA) item. Potential statuses include:\\n\\n* SUCCESSFUL - The DPA is eligible to process transactions.\\n\\n* FAILED - The DPA is NOT eligible to process\
  \ transactions. Please see the error object for more details.\\\"\\n\"\n    },\n    \"dpaName\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of Merchant (which may differ from dpaPresentationName).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-dpa-results-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DpaResults
---
