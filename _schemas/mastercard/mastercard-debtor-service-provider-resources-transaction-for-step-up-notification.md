---
description: ''
layout: schema
name: TransactionForStepUpNotification
properties_list:
- description: Unique identifier assigned by Mastercard, to identify the payment request in subsequent transactions or services.
  name: paymentRequestLifecycleId
  type: string
- description: Text message that DSP will be providing to display to the Debtor on Creditor website or application.
  name: stepUpMessage
  type: string
- description: URL that will be used by the Debtor to open the banking app from Creditor's website or application on a single device journey. Creditor should only use this when it's a single device journey.
  name: applicationUrl
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-transaction-for-step-up-notification-schema.json
slug: mastercard-debtor-service-provider-resources-transaction-for-step-up-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionForStepUpNotification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentRequestLifecycleId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by Mastercard, to identify the payment request in subsequent transactions or services.\"\n    },\n    \"stepUpMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Text message that DSP will be providing to display to the Debtor on Creditor website or application.\"\n    },\n    \"applicationUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL that will be used by the Debtor to open the banking app from Creditor's website or application on a single device journey. Creditor should only use this when it's a single device journey.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-transaction-for-step-up-notification-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: TransactionForStepUpNotification
---
