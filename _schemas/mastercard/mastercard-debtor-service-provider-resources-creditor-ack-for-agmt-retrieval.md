---
description: ''
layout: schema
name: CreditorAckForAgmtRetrieval
properties_list:
- description: Unique identifier assigned to the Creditor by the CSP.
  name: creditorId
  type: string
- description: Unique identifier assigned to the CSP during Mastercard onboarding.
  name: creditorServiceProviderId
  type: string
- description: Name used by the Creditor in dealing with customers, which may not be the same as the one it uses for legal purposes.
  name: creditorTradeName
  type: string
- description: The category code of the Creditor, also known as Merchant Category Code (MCC). Enables the classification of Creditors into specific categories based on the type of business, trade or services supplie
  name: creditorCategoryCode
  type: string
- description: Creditor's Logo (in URL encoded format). Can be used by the Debtor to display the Creditor's Logo.
  name: creditorLogoUrl
  type: string
- description: Return string (in URL encoded format) that is passed to the DSP to return the Debtor back to the Creditor's page.
  name: creditorReturnString
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-creditor-ack-for-agmt-retrieval-schema.json
slug: mastercard-debtor-service-provider-resources-creditor-ack-for-agmt-retrieval
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreditorAckForAgmtRetrieval\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the Creditor by the CSP.\"\n    },\n    \"creditorServiceProviderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the CSP during Mastercard onboarding.\"\n    },\n    \"creditorTradeName\": {\n      \"type\": \"string\",\n      \"description\": \"Name used by the Creditor in dealing with customers,  which may not be the same as the one it uses for legal purposes.\"\n    },\n    \"creditorCategoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"The category code of the Creditor, also known as Merchant Category Code (MCC). Enables the classification of Creditors into specific categories based on the type of business, trade or services supplied.\"\n    },\n\
  \    \"creditorLogoUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Creditor's Logo (in URL encoded format). Can be used by the Debtor to display the Creditor's Logo.\"\n    },\n    \"creditorReturnString\": {\n      \"type\": \"string\",\n      \"description\": \"Return string (in URL encoded format) that is passed to the DSP to return the Debtor back to the Creditor's page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-creditor-ack-for-agmt-retrieval-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CreditorAckForAgmtRetrieval
---
