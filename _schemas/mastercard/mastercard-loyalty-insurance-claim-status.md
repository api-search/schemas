---
description: ''
layout: schema
name: ClaimStatus
properties_list:
- description: Array of insurance claim features associated with the claim.
  name: features
  type: array
- description: URL to web page that facilitates uploading documents.
  name: uploadDocumentsUrl
  type: string
- description: Array of required documents for this claim.
  name: requiredDocuments
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-loyalty-insurance-claim-status-schema.json
slug: mastercard-loyalty-insurance-claim-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClaimStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"Array of insurance claim features associated with the claim.\"\n    },\n    \"uploadDocumentsUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to web page that facilitates uploading documents.\"\n    },\n    \"requiredDocuments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of required documents for this claim.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-loyalty-insurance-claim-status-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ClaimStatus
---
