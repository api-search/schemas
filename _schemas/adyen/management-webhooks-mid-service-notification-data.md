---
description: MidServiceNotificationData schema from Adyen API
layout: schema
name: MidServiceNotificationData
properties_list:
- description: Indicates whether receiving payments is allowed. This value is set to **true** by Adyen after screening your merchant account.
  name: allowed
  type: boolean
- description: Indicates whether the payment method is enabled (**true**) or disabled (**false**).
  name: enabled
  type: boolean
- description: The unique identifier of the resource.
  name: id
  type: string
- description: The unique identifier of the merchant account.
  name: merchantId
  type: string
- description: Your reference for the payment method.
  name: reference
  type: string
- description: 'The status of the request to add a payment method. Possible values: * **success**: the payment method was added. * **failure**: the request failed. * **capabilityPending**: the **receivePayments** cap'
  name: status
  type: string
- description: The unique identifier of the [store](https://docs.adyen.com/api-explorer/#/ManagementService/latest/post/merchants/{id}/paymentMethodSettings__reqParam_storeId), if any.
  name: storeId
  type: string
- description: Payment method [variant](https://docs.adyen.com/development-resources/paymentmethodvariant#management-api).
  name: type
  type: string
- description: 'Payment method status. Possible values: * **valid** * **pending** * **invalid** * **rejected**'
  name: verificationStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhooks-mid-service-notification-data-schema.json
slug: management-webhooks-mid-service-notification-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-mid-service-notification-data-schema.json\",\n  \"title\": \"MidServiceNotificationData\",\n  \"description\": \"MidServiceNotificationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed\": {\n      \"description\": \"Indicates whether receiving payments is allowed. This value is set to **true** by Adyen after screening your merchant account.\",\n      \"type\": \"boolean\"\n    },\n    \"enabled\": {\n      \"description\": \"Indicates whether the payment method is enabled (**true**) or disabled (**false**).\",\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the resource.\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The unique identifier of the merchant account.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the payment method.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The status of the request to add a payment method. Possible values:\\n\\n* **success**: the payment method was added.\\n* **failure**: the request failed.\\n* **capabilityPending**: the **receivePayments** capability is not allowed.\\n\",\n      \"enum\": [\n        \"success\",\n        \"failure\",\n        \"capabilityPending\",\n        \"dataRequired\",\n        \"updatesExpected\"\n      ],\n      \"type\": \"string\"\n    },\n    \"storeId\": {\n      \"description\": \"The unique identifier of the [store](https://docs.adyen.com/api-explorer/#/ManagementService/latest/post/merchants/{id}/paymentMethodSettings__reqParam_storeId), if any.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Payment method [variant](https://docs.adyen.com/development-resources/paymentmethodvariant#management-api).\"\
  ,\n      \"type\": \"string\"\n    },\n    \"verificationStatus\": {\n      \"description\": \"Payment method status. Possible values:\\n* **valid**\\n* **pending**\\n* **invalid**\\n* **rejected**\",\n      \"enum\": [\n        \"valid\",\n        \"pending\",\n        \"invalid\",\n        \"rejected\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"merchantId\",\n    \"id\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-mid-service-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MidServiceNotificationData
---
