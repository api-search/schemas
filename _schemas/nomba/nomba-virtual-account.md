---
description: Schema representing a Nomba virtual bank account used for collecting payments via bank transfers.
layout: schema
name: Nomba Virtual Account
properties_list:
- description: The unique reference identifier for the virtual account.
  name: accountRef
  type: string
- description: The name associated with the virtual account, typically the customer name.
  name: accountName
  type: string
- description: The bank account number assigned to the virtual account.
  name: accountNumber
  type: string
- description: The name of the bank providing the virtual account number.
  name: bankName
  type: string
- description: The bank code of the issuing bank.
  name: bankCode
  type: string
- description: The current status of the virtual account.
  name: status
  type: string
- description: The date and time the virtual account expires and stops accepting payments.
  name: expiryDate
  type: string
- description: The date and time the virtual account was created.
  name: createdAt
  type: string
- description: The date and time the virtual account was last updated.
  name: updatedAt
  type: string
provider_name: Nomba
provider_slug: nomba
schema_file: json-schema/nomba-virtual-account-schema.json
slug: nomba-virtual-account
source_filename: nomba-virtual-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.nomba.com/schemas/nomba/virtual-account.json\",\n  \"title\": \"Nomba Virtual Account\",\n  \"description\": \"Schema representing a Nomba virtual bank account used for collecting payments via bank transfers.\",\n  \"type\": \"object\",\n  \"required\": [\"accountRef\", \"accountName\", \"accountNumber\"],\n  \"properties\": {\n    \"accountRef\": {\n      \"type\": \"string\",\n      \"description\": \"The unique reference identifier for the virtual account.\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"The name associated with the virtual account, typically the customer name.\",\n      \"minLength\": 1,\n      \"maxLength\": 200\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The bank account number assigned to the virtual account.\",\n      \"pattern\": \"^\\\\d{10}$\"\n    },\n    \"bankName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The name of the bank providing the virtual account number.\"\n    },\n    \"bankCode\": {\n      \"type\": \"string\",\n      \"description\": \"The bank code of the issuing bank.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the virtual account.\",\n      \"enum\": [\"active\", \"expired\"]\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the virtual account expires and stops accepting payments.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the virtual account was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the virtual account was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/json-schema/nomba-virtual-account-schema.json
tags:
- Payments
- Fintech
- Banking
- Transfers
- Virtual Accounts
- Checkout
- Cross-Border Payments
- Cards
title: Nomba Virtual Account
---
