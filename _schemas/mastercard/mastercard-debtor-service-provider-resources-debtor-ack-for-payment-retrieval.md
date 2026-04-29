---
description: ''
layout: schema
name: DebtorAckForPaymentRetrieval
properties_list:
- description: Unique identifier of the Debtor provided to Mastercard by the DSP.
  name: debtorId
  type: string
- description: Unique identifier assigned to the DSP during Mastercard onboarding.
  name: debtorServiceProviderId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-debtor-ack-for-payment-retrieval-schema.json
slug: mastercard-debtor-service-provider-resources-debtor-ack-for-payment-retrieval
source_filename: mastercard-debtor-service-provider-resources-debtor-ack-for-payment-retrieval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DebtorAckForPaymentRetrieval\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"debtorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the Debtor provided to Mastercard by the DSP.\"\n    },\n    \"debtorServiceProviderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the DSP during Mastercard onboarding.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-debtor-ack-for-payment-retrieval-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DebtorAckForPaymentRetrieval
---
