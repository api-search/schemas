---
description: ''
layout: schema
name: Creditor
properties_list:
- description: Unique identifier assigned to the CSP during Mastercard onboarding.
  name: creditorServiceProviderId
  type: string
- description: Unique identifier assigned to the Creditor by the CSP.
  name: creditorId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-creditor-schema.json
slug: mastercard-debtor-service-provider-resources-creditor
source_filename: mastercard-debtor-service-provider-resources-creditor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Creditor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditorServiceProviderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the CSP during Mastercard onboarding.\"\n    },\n    \"creditorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the Creditor by the CSP.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-creditor-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Creditor
---
