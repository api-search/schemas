---
description: Legal document that is required for KYC.
layout: schema
name: LegalDocument
properties_list:
- description: ID of legal document. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when legal document type is provided.
  name: id
  type: string
- description: 'Place of issuance of legal document <BR/> **Conditional Mandatory**<font color=''red''>* </font> field - Required when legal document id is provided and configured in document checklist plan associated '
  name: placeOfIssuance
  type: string
- description: Date on which the legal document will expire. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when legal document id is provided and configured in document checklist plan a
  name: expiryDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-legal-document-schema.json
slug: mastercard-card-issuance-legal-document
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LegalDocument\",\n  \"type\": \"object\",\n  \"description\": \"Legal document that is required for KYC.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of legal document. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when legal document type is provided.\"\n    },\n    \"placeOfIssuance\": {\n      \"type\": \"string\",\n      \"description\": \"Place of issuance of legal document <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when legal document id is provided and configured in document checklist plan associated with program.\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date on which the legal document will expire. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required when legal document id is provided and configured in\
  \ document checklist plan associated with program. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-legal-document-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: LegalDocument
---
