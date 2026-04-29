---
description: TransactionList schema from Amazon Selling Partner API
layout: schema
name: TransactionList
properties_list:
- description: ''
  name: transactions
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-transaction-list-schema.json
slug: selling-partner-transaction-list
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"transactionType\": {\n            \"type\": \"string\"\n          },\n          \"transactionId\": {\n            \"type\": \"string\"\n          },\n          \"transactionStatus\": {\n            \"type\": \"string\"\n          },\n          \"postedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"totalAmount\": {\n            \"$ref\": \"#/components/schemas/Money\"\n          }\n        }\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionList\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-transaction-list-schema.json\",\n  \"description\"\
  : \"TransactionList schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-transaction-list-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: TransactionList
---
