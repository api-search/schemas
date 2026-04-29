---
description: ''
layout: schema
name: Account
properties_list:
- description: ''
  name: id
  type: string
- description: The account number
  name: number
  type: string
- description: The account display name
  name: displayName
  type: string
- description: The account category
  name: category
  type: string
- description: The account subcategory
  name: subCategory
  type: string
- description: Whether the account is blocked
  name: blocked
  type: boolean
- description: The account type
  name: accountType
  type: string
- description: Whether direct posting is allowed
  name: directPosting
  type: boolean
- description: The net change
  name: netChange
  type: number
- description: ''
  name: consolidationTranslationMethod
  type: string
- description: ''
  name: consolidationDebitAccount
  type: string
- description: ''
  name: consolidationCreditAccount
  type: string
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-account-schema.json
slug: business-central-v2-account
source_filename: business-central-v2-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The account number\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The account display name\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The account category\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The account subcategory\"\n    },\n    \"blocked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account is blocked\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"The account type\"\n    },\n    \"directPosting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether direct posting is allowed\"\n    },\n    \"netChange\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"The net change\"\n    },\n    \"consolidationTranslationMethod\": {\n      \"type\": \"string\"\n    },\n    \"consolidationDebitAccount\": {\n      \"type\": \"string\"\n    },\n    \"consolidationCreditAccount\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-account-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Account
---
