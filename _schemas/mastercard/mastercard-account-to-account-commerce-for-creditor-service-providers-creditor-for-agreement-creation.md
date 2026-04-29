---
description: ''
layout: schema
name: CreditorForAgreementCreation
properties_list:
- description: Unique identifier assigned to the Creditor by the CSP.
  name: creditorId
  type: string
- description: Unique identifier assigned to the CSP during Mastercard onboarding.
  name: creditorServiceProviderId
  type: string
- description: Return string (in URL encoded format) that is passed to the DSP to return the Debtor back to the Creditor's checkout page.
  name: creditorReturnString
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-creditor-for-agreement-creation-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-creditor-for-agreement-creation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreditorForAgreementCreation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the Creditor by the CSP.\"\n    },\n    \"creditorServiceProviderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the CSP during Mastercard onboarding.\"\n    },\n    \"creditorReturnString\": {\n      \"type\": \"string\",\n      \"description\": \"Return string (in URL encoded format) that is passed to the DSP to return the Debtor back to the Creditor's checkout page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-creditor-for-agreement-creation-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CreditorForAgreementCreation
---
