---
description: CardDetails schema from Adyen API
layout: schema
name: CardDetails
properties_list:
- description: 'Secondary brand of the card. For example: **plastix**, **hmclub**.'
  name: brand
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: ''
  name: cupsecureplus.smscode
  type: string
- description: The card verification code. Only collect raw card data if you are [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).
  name: cvc
  type: string
- description: The encrypted card number.
  name: encryptedCardNumber
  type: string
- description: The encrypted card expiry month.
  name: encryptedExpiryMonth
  type: string
- description: The encrypted card expiry year.
  name: encryptedExpiryYear
  type: string
- description: The encrypted card verification code.
  name: encryptedSecurityCode
  type: string
- description: The card expiry month. Only collect raw card data if you are [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).
  name: expiryMonth
  type: string
- description: The card expiry year. Only collect raw card data if you are [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).
  name: expiryYear
  type: string
- description: The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.
  name: fundingSource
  type: string
- description: The name of the card holder.
  name: holderName
  type: string
- description: The network token reference. This is the [`networkTxReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_additionalData-ResponseAdditionalDataCommon-network
  name: networkPaymentReference
  type: string
- description: The card number. Only collect raw card data if you are [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).
  name: number
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: The `shopperNotificationReference` returned in the response when you requested to notify the shopper. Used only for recurring payments in India.
  name: shopperNotificationReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: Required for mobile integrations. Version of the 3D Secure 2 mobile SDK.
  name: threeDS2SdkVersion
  type: string
- description: Default payment method details. Common for scheme payment methods, and for simple payment method details.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-card-details-schema.json
slug: checkout-card-details
source_filename: checkout-card-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-details-schema.json\",\n  \"title\": \"CardDetails\",\n  \"description\": \"CardDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"description\": \"Secondary brand of the card. For example: **plastix**, **hmclub**.\",\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"cupsecureplus.smscode\": {\n      \"deprecated\": true,\n      \"type\": \"string\"\n    },\n    \"cvc\": {\n      \"description\": \"The card verification code. Only collect raw card data if you are [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).\",\n      \"type\": \"string\"\n \
  \   },\n    \"encryptedCardNumber\": {\n      \"description\": \"The encrypted card number.\",\n      \"maxLength\": 15000,\n      \"type\": \"string\"\n    },\n    \"encryptedExpiryMonth\": {\n      \"description\": \"The encrypted card expiry month.\",\n      \"maxLength\": 15000,\n      \"type\": \"string\"\n    },\n    \"encryptedExpiryYear\": {\n      \"description\": \"The encrypted card expiry year.\",\n      \"maxLength\": 15000,\n      \"type\": \"string\"\n    },\n    \"encryptedSecurityCode\": {\n      \"description\": \"The encrypted card verification code.\",\n      \"maxLength\": 15000,\n      \"type\": \"string\"\n    },\n    \"expiryMonth\": {\n      \"description\": \"The card expiry month. Only collect raw card data if you are [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).\",\n      \"type\": \"string\"\n    },\n    \"expiryYear\": {\n      \"description\": \"The card expiry year. Only collect raw card data if you are [fully\
  \ PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).\",\n      \"type\": \"string\"\n    },\n    \"fundingSource\": {\n      \"description\": \"The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.\",\n      \"enum\": [\n        \"credit\",\n        \"debit\"\n      ],\n      \"type\": \"string\"\n    },\n    \"holderName\": {\n      \"description\": \"The name of the card holder.\",\n      \"type\": \"string\"\n    },\n    \"networkPaymentReference\": {\n      \"description\": \"The network token reference. This is the [`networkTxReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_additionalData-ResponseAdditionalDataCommon-networkTxReference) from the response to the first payment.\",\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"description\": \"The card\
  \ number. Only collect raw card data if you are [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide).\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"shopperNotificationReference\": {\n      \"description\": \"The `shopperNotificationReference` returned in the response when you requested to notify the shopper. Used only for recurring payments in India.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\"\
  : \"string\"\n    },\n    \"threeDS2SdkVersion\": {\n      \"description\": \"Required for mobile integrations. Version of the 3D Secure 2 mobile SDK.\",\n      \"maxLength\": 12,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"scheme\",\n      \"description\": \"Default payment method details. Common for scheme payment methods, and for simple payment method details.\",\n      \"enum\": [\n        \"bcmc\",\n        \"scheme\",\n        \"networkToken\",\n        \"giftcard\",\n        \"card\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardDetails
---
