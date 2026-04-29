---
description: AccountCreateNotificationData schema from Adyen API
layout: schema
name: AccountCreateNotificationData
properties_list:
- description: Key-value pairs that specify the actions that the merchant account can do and its settings. The key is a capability. For example, the **sendToTransferInstrument** is the capability required before you
  name: capabilities
  type: object
- description: The unique identifier of the company account.
  name: companyId
  type: string
- description: The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id).
  name: legalEntityId
  type: string
- description: The unique identifier of the merchant account.
  name: merchantId
  type: string
- description: 'The status of the merchant account. Possible values: * **PreActive**: The merchant account has been created. Users cannot access the merchant account in the Customer Area. The account cannot process p'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhooks-account-create-notification-data-schema.json
slug: management-webhooks-account-create-notification-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-account-create-notification-data-schema.json\",\n  \"title\": \"AccountCreateNotificationData\",\n  \"description\": \"AccountCreateNotificationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AccountCapabilityData\"\n      },\n      \"description\": \"Key-value pairs that specify the actions that the merchant account can do and its settings. The key is a capability. For example, the **sendToTransferInstrument** is the capability required before you can pay out funds to the bank account. The value is an object containing the settings for the capability.\",\n      \"type\": \"object\"\n    },\n    \"companyId\": {\n      \"description\": \"The unique identifier of the\
  \ company account.\",\n      \"type\": \"string\"\n    },\n    \"legalEntityId\": {\n      \"description\": \"The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id).\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The unique identifier of the merchant account.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the merchant account.\\n\\nPossible values:\\n\\n* **PreActive**: The merchant account has been created. Users cannot access the merchant account in the Customer Area. The account cannot process payments.\\n* **Active**: Users can access the merchant account in the Customer Area. If the company account is also **Active**, then payment processing and payouts are enabled.\\n* **InactiveWithModifications**: Users can access the merchant account in the Customer Area. The account cannot process new payments but can still\
  \ modify payments, for example issue refunds. The account can still receive payouts.\\n* **Inactive**: Users can access the merchant account in the Customer Area. Payment processing and payouts are disabled.\\n* **Closed**: The account is closed and this cannot be reversed. Users cannot log in. Payment processing and payouts are disabled.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantId\",\n    \"companyId\",\n    \"status\",\n    \"capabilities\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-account-create-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountCreateNotificationData
---
