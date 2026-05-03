---
description: A SaaS contract managed within the Torii platform, including renewal and cost information.
layout: schema
name: Torii Contract
properties_list:
- description: Unique identifier for the contract.
  name: id
  type: string
- description: Associated application ID.
  name: appId
  type: string
- description: Associated application name.
  name: appName
  type: string
- description: Contract name.
  name: name
  type: string
- description: Contract status.
  name: status
  type: string
- description: Contract start date.
  name: startDate
  type: string
- description: Contract end date.
  name: endDate
  type: string
- description: Contract renewal date.
  name: renewalDate
  type: string
- description: Annual cost.
  name: annualCost
  type: number
- description: Currency code.
  name: currency
  type: string
- description: Contract owner.
  name: owner
  type: string
- description: When the contract was created.
  name: createdAt
  type: string
provider_name: Torii
provider_slug: torii
schema_file: json-schema/contract.json
slug: contract
source_filename: contract.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/contract.json\",\n  \"title\": \"Torii Contract\",\n  \"description\": \"A SaaS contract managed within the Torii platform, including renewal and cost information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the contract.\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated application ID.\"\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated application name.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Contract name.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Contract status.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date\",\n      \"description\": \"Contract start date.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Contract end date.\"\n    },\n    \"renewalDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Contract renewal date.\"\n    },\n    \"annualCost\": {\n      \"type\": \"number\",\n      \"description\": \"Annual cost.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Contract owner.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the contract was created.\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/contract.json
tags:
- SaaS Management
title: Torii Contract
---
