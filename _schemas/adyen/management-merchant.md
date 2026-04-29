---
description: Merchant schema from Adyen API
layout: schema
name: Merchant
properties_list:
- description: References to resources connected with this merchant.
  name: _links
  type: object
- description: 'The [capture delay](https://docs.adyen.com/online-payments/capture#capture-delay) set for the merchant account. Possible values: * **Immediate** * **Manual** * Number of days from **1** to **29**'
  name: captureDelay
  type: string
- description: The unique identifier of the company account this merchant belongs to
  name: companyId
  type: string
- description: List of available data centers. Adyen has several data centers around the world.In the URL that you use for making API requests, we recommend you use the live URL prefix from the data center closest t
  name: dataCenters
  type: array
- description: The default [`shopperInteraction`](https://docs.adyen.com/api-explorer/#/CheckoutService/v68/post/payments__reqParam_shopperInteraction) value used when processing payments through this merchant accou
  name: defaultShopperInteraction
  type: string
- description: Your description for the merchant account, maximum 300 characters
  name: description
  type: string
- description: The unique identifier of the merchant account.
  name: id
  type: string
- description: The city where the legal entity of this merchant account is registered.
  name: merchantCity
  type: string
- description: The name of the legal entity associated with the merchant account.
  name: name
  type: string
- description: Only applies to merchant accounts managed by Adyen's partners. The name of the pricing plan assigned to the merchant account.
  name: pricingPlan
  type: string
- description: 'The currency of the country where the legal entity of this merchant account is registered. Format: [ISO currency code](https://docs.adyen.com/development-resources/currency-codes). For example, a lega'
  name: primarySettlementCurrency
  type: string
- description: Reference of the merchant account.
  name: reference
  type: string
- description: The URL for the ecommerce website used with this merchant account.
  name: shopWebAddress
  type: string
- description: 'The status of the merchant account. Possible values: * **PreActive**: The merchant account has been created. Users cannot access the merchant account in the Customer Area. The account cannot process p'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-merchant-schema.json
slug: management-merchant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-merchant-schema.json\",\n  \"title\": \"Merchant\",\n  \"description\": \"Merchant schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"References to resources connected with this merchant.\",\n      \"$ref\": \"#/components/schemas/MerchantLinks\"\n    },\n    \"captureDelay\": {\n      \"description\": \"The [capture delay](https://docs.adyen.com/online-payments/capture#capture-delay) set for the merchant account.\\n\\nPossible values:\\n* **Immediate**\\n* **Manual**\\n* Number of days from **1** to **29**\",\n      \"type\": \"string\"\n    },\n    \"companyId\": {\n      \"description\": \"The unique identifier of the company account this merchant belongs to\",\n      \"type\": \"string\"\n    },\n    \"dataCenters\": {\n      \"description\"\
  : \"List of available data centers.\\n\\nAdyen has several data centers around the world.In the URL that you use for making API requests, we recommend you use the live URL prefix from the data center closest to your shoppers.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DataCenter\"\n      },\n      \"type\": \"array\"\n    },\n    \"defaultShopperInteraction\": {\n      \"description\": \"The default [`shopperInteraction`](https://docs.adyen.com/api-explorer/#/CheckoutService/v68/post/payments__reqParam_shopperInteraction) value used when processing payments through this merchant account.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the merchant account, maximum 300 characters\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the merchant account.\",\n      \"type\": \"string\"\n    },\n    \"merchantCity\": {\n      \"description\": \"The city where\
  \ the legal entity of this merchant account is registered.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the legal entity associated with the merchant account.\",\n      \"type\": \"string\"\n    },\n    \"pricingPlan\": {\n      \"description\": \"Only applies to merchant accounts managed by Adyen's partners. The name of the pricing plan assigned to the merchant account.\",\n      \"type\": \"string\"\n    },\n    \"primarySettlementCurrency\": {\n      \"description\": \"The currency of the country where the legal entity of this merchant account is registered. Format: [ISO currency code](https://docs.adyen.com/development-resources/currency-codes). For example, a legal entity based in the United States has USD as the primary settlement currency.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Reference of the merchant account.\",\n      \"type\": \"string\"\n    },\n    \"shopWebAddress\": {\n    \
  \  \"description\": \"The URL for the ecommerce website used with this merchant account.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the merchant account.\\n\\nPossible values:\\n\\n* **PreActive**: The merchant account has been created. Users cannot access the merchant account in the Customer Area. The account cannot process payments.\\n* **Active**: Users can access the merchant account in the Customer Area. If the company account is also **Active**, then payment processing and payouts are enabled.\\n* **InactiveWithModifications**: Users can access the merchant account in the Customer Area. You cannot process new payments but you can still modify payments, for example issue refunds. You can still receive payouts.\\n* **Inactive**: Users can access the merchant account in the Customer Area. Payment processing and payouts are disabled.\\n* **Closed**: The account is closed and this cannot be reversed. Users cannot log in. Payment processing\
  \ and payouts are disabled.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-merchant-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Merchant
---
