---
description: TransactionParty schema from Avalara API
layout: schema
name: TransactionParty
properties_list:
- description: ''
  name: companyId
  type: string
- description: ''
  name: locationId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: licenseNumber
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-transaction-party-schema.json
slug: excise-transaction-party
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-transaction-party-schema.json\",\n  \"title\": \"TransactionParty\",\n  \"description\": \"TransactionParty schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"locationId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/ExciseAddress\"\n    },\n    \"licenseNumber\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-transaction-party-schema.json
tags:
- Taxes
title: TransactionParty
---
