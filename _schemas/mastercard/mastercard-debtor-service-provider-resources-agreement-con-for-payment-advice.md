---
description: Agreement Confirmation from DSP
layout: schema
name: AgreementConForPaymentAdvice
properties_list:
- description: Indicates true whether Agreement was confirmed by Debtor. False for any other reasons.
  name: agreementConfirmed
  type: boolean
- description: Reason for declined agreement. * Refer to Codes and Formats section for more details.
  name: agreementStatusReason
  type: string
- description: Nickname of the account is passed when agreementConfirmed is true.
  name: accountNickname
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-agreement-con-for-payment-advice-schema.json
slug: mastercard-debtor-service-provider-resources-agreement-con-for-payment-advice
source_filename: mastercard-debtor-service-provider-resources-agreement-con-for-payment-advice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgreementConForPaymentAdvice\",\n  \"type\": \"object\",\n  \"description\": \"Agreement Confirmation from DSP\",\n  \"properties\": {\n    \"agreementConfirmed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates true whether Agreement was confirmed by Debtor. False for any other reasons.\"\n    },\n    \"agreementStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for declined agreement. * Refer to Codes and Formats section for more details.\"\n    },\n    \"accountNickname\": {\n      \"type\": \"string\",\n      \"description\": \"Nickname of the account is passed when agreementConfirmed is true.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-agreement-con-for-payment-advice-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AgreementConForPaymentAdvice
---
