---
description: StoreSplitConfiguration schema from Adyen API
layout: schema
name: StoreSplitConfiguration
properties_list:
- description: The [unique identifier of the balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balanceAccounts/{id}__queryParam_id) to which the split amount must be booked, depending
  name: balanceAccountId
  type: string
- description: The unique identifier of the [split configuration profile](https://docs.adyen.com/marketplaces-and-platforms/automatic-split-configuration/create-split-configuration/).
  name: splitConfigurationId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-store-split-configuration-schema.json
slug: management-store-split-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-store-split-configuration-schema.json\",\n  \"title\": \"StoreSplitConfiguration\",\n  \"description\": \"StoreSplitConfiguration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The [unique identifier of the balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balanceAccounts/{id}__queryParam_id) to which the split amount must be booked, depending on the defined [split logic](https://docs.adyen.com/api-explorer/Management/latest/post/merchants/_merchantId_/splitConfigurations#request-rules-splitLogic).\",\n      \"type\": \"string\"\n    },\n    \"splitConfigurationId\": {\n      \"description\": \"The unique identifier of the [split configuration profile](https://docs.adyen.com/marketplaces-and-platforms/automatic-split-configuration/create-split-configuration/).\"\
  ,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-store-split-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoreSplitConfiguration
---
