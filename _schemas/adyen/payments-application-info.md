---
description: ApplicationInfo schema from Adyen API
layout: schema
name: ApplicationInfo
properties_list:
- description: Adyen-developed software, such as libraries and plugins, used to interact with the Adyen API. For example, Magento plugin, Java API library, etc.
  name: adyenLibrary
  type: object
- description: Adyen-developed software to get payment details. For example, Checkout SDK, Secured Fields SDK, etc.
  name: adyenPaymentSource
  type: object
- description: Third-party developed platform used to initiate payment requests. For example, Magento, Zuora, etc.
  name: externalPlatform
  type: object
- description: Merchant developed software, such as cashier application, used to interact with the Adyen API.
  name: merchantApplication
  type: object
- description: Merchant device information.
  name: merchantDevice
  type: object
- description: Shopper interaction device, such as terminal, mobile device or web browser, to initiate payment requests.
  name: shopperInteractionDevice
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-application-info-schema.json
slug: payments-application-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-application-info-schema.json\",\n  \"title\": \"ApplicationInfo\",\n  \"description\": \"ApplicationInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adyenLibrary\": {\n      \"description\": \"Adyen-developed software, such as libraries and plugins, used to interact with the Adyen API. For example, Magento plugin, Java API library, etc.\",\n      \"$ref\": \"#/components/schemas/CommonField\"\n    },\n    \"adyenPaymentSource\": {\n      \"description\": \"Adyen-developed software to get payment details. For example, Checkout SDK, Secured Fields SDK, etc.\",\n      \"$ref\": \"#/components/schemas/CommonField\"\n    },\n    \"externalPlatform\": {\n      \"description\": \"Third-party developed platform used to initiate payment requests. For example, Magento, Zuora, etc.\"\
  ,\n      \"$ref\": \"#/components/schemas/ExternalPlatform\"\n    },\n    \"merchantApplication\": {\n      \"description\": \"Merchant developed software, such as cashier application, used to interact with the Adyen API.\",\n      \"$ref\": \"#/components/schemas/CommonField\"\n    },\n    \"merchantDevice\": {\n      \"description\": \"Merchant device information.\",\n      \"$ref\": \"#/components/schemas/MerchantDevice\"\n    },\n    \"shopperInteractionDevice\": {\n      \"description\": \"Shopper interaction device, such as terminal, mobile device or web browser, to initiate payment requests.\",\n      \"$ref\": \"#/components/schemas/ShopperInteractionDevice\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-application-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ApplicationInfo
---
