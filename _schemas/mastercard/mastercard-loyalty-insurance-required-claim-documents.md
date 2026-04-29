---
description: ''
layout: schema
name: RequiredClaimDocuments
properties_list:
- description: Name of the document required for an insurance claim.
  name: name
  type: string
- description: Description of the document required for an insurance claim.
  name: description
  type: string
- description: Received indicator of the insurance claim document.
  name: isReceived
  type: boolean
- description: Category of the document required for an insurance claim.
  name: category
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-loyalty-insurance-required-claim-documents-schema.json
slug: mastercard-loyalty-insurance-required-claim-documents
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequiredClaimDocuments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the document required for an insurance claim.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the document required for an insurance claim.\"\n    },\n    \"isReceived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Received indicator of the insurance claim document.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the document required for an insurance claim.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-loyalty-insurance-required-claim-documents-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: RequiredClaimDocuments
---
