---
description: Transaction schema from Adyen API
layout: schema
name: Transaction
properties_list:
- description: Contains information about the account holder associated with the `balanceAccount`.
  name: accountHolder
  type: object
- description: Contains information about the amount of the transaction.
  name: amount
  type: object
- description: Contains information about the balance account involved in the transaction.
  name: balanceAccount
  type: object
- description: The unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: The date the transaction was booked into the balance account.
  name: bookingDate
  type: string
- description: The date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.
  name: creationDate
  type: string
- description: The unique identifier of the transaction.
  name: id
  type: string
- description: 'The status of the transaction. Possible values: * **pending**: The transaction is still pending. * **booked**: The transaction has been booked to the balance account.'
  name: status
  type: string
- description: Contains information about the transfer related to the transaction.
  name: transfer
  type: object
- description: The date the transfer amount becomes available in the balance account.
  name: valueDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-transaction-schema.json
slug: transfers-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"Transaction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Contains information about the account holder associated with the `balanceAccount`.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"amount\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"Contains information about the amount of the transaction.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"balanceAccount\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Contains information about the balance account involved in the transaction.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\
  \n    },\n    \"balancePlatform\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"bookingDate\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The date the transaction was booked into the balance account.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"description\": \"The date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The unique identifier of the transaction.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The status of the transaction.\\n\\n Possible values:\\n\\n* **pending**: The transaction is still pending.\\\
  n\\n* **booked**: The transaction has been booked to the balance account.\\n\\n\",\n      \"enum\": [\n        \"booked\",\n        \"pending\"\n      ],\n      \"type\": \"string\"\n    },\n    \"transfer\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Contains information about the transfer related to the transaction.\",\n      \"$ref\": \"#/components/schemas/TransferData\"\n    },\n    \"valueDate\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The date the transfer amount becomes available in the balance account.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"accountHolder\",\n    \"balanceAccount\",\n    \"amount\",\n    \"status\",\n    \"bookingDate\",\n    \"valueDate\",\n    \"balancePlatform\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transaction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Transaction
---
