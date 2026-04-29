---
description: BankCategoryData schema from Adyen API
layout: schema
name: BankCategoryData
properties_list:
- description: 'The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Required for transfers with `category` **bank**. Possible values: * **regular**'
  name: priority
  type: string
- description: '**bank**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-bank-category-data-schema.json
slug: transfer-webhooks-bank-category-data
source_filename: transfer-webhooks-bank-category-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-bank-category-data-schema.json\",\n  \"title\": \"BankCategoryData\",\n  \"description\": \"BankCategoryData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"priority\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Required for transfers with `category` **bank**.\\n\\nPossible values:\\n\\n* **regular**: For normal, low-value transactions.\\n\\n* **fast**: Faster way to transfer funds but has higher fees. Recommended for high-priority, low-value transactions.\\n\\n* **wire**: Fastest way to transfer funds but has the highest fees. Recommended for high-priority, high-value transactions.\\n\\n* **instant**: Instant way to transfer\
  \ funds in [SEPA countries](https://www.ecb.europa.eu/paym/integration/retail/sepa/html/index.en.html).\\n\\n* **crossBorder**: High-value transfer to a recipient in a different country.\\n\\n* **internal**: Transfer to an Adyen-issued business bank account (by bank account number/IBAN).\",\n      \"enum\": [\n        \"crossBorder\",\n        \"fast\",\n        \"instant\",\n        \"internal\",\n        \"regular\",\n        \"wire\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"bank\",\n      \"description\": \"**bank**\",\n      \"enum\": [\n        \"bank\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-bank-category-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankCategoryData
---
