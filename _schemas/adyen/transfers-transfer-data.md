---
description: TransferData schema from Adyen API
layout: schema
name: TransferData
properties_list:
- description: The ID of the resource.
  name: id
  type: string
- description: The [`reference`](https://docs.adyen.com/api-explorer/#/transfers/latest/post/transfers__reqParam_reference) from the `/transfers` request. If you haven't provided any, Adyen generates a unique refere
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-transfer-data-schema.json
slug: transfers-transfer-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-data-schema.json\",\n  \"title\": \"TransferData\",\n  \"description\": \"TransferData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The ID of the resource.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The [`reference`](https://docs.adyen.com/api-explorer/#/transfers/latest/post/transfers__reqParam_reference) from the `/transfers` request. If you haven't provided any, Adyen generates a unique reference.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"reference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferData
---
