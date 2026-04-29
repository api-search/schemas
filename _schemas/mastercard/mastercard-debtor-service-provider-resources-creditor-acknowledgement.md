---
description: ''
layout: schema
name: CreditorAcknowledgement
properties_list:
- description: Unique identifier assigned to the Creditor by the CSP.
  name: creditorId
  type: string
- description: Name used by the Creditor in dealing with customers, which may not be the same as the one it uses for legal purposes.
  name: creditorTradeName
  type: string
- description: Creditor's Logo (in URL encoded format). Can be used by the Debtor to display the Creditor's Logo.
  name: creditorLogoUrl
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-creditor-acknowledgement-schema.json
slug: mastercard-debtor-service-provider-resources-creditor-acknowledgement
source_filename: mastercard-debtor-service-provider-resources-creditor-acknowledgement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreditorAcknowledgement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the Creditor by the CSP.\"\n    },\n    \"creditorTradeName\": {\n      \"type\": \"string\",\n      \"description\": \"Name used by the Creditor in dealing with customers, which may not be the same as the one it uses for legal purposes.\"\n    },\n    \"creditorLogoUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Creditor's Logo (in URL encoded format). Can be used by the Debtor to display the Creditor's Logo.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-creditor-acknowledgement-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CreditorAcknowledgement
---
