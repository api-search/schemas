---
description: Normalized deal/opportunity entity returned by the Revert Unified CRM API
layout: schema
name: Revert Unified CRM Deal
properties_list:
- description: Revert-normalized unique deal identifier
  name: id
  type: string
- description: The original ID from the source CRM provider
  name: remoteId
  type: string
- description: Deal name or title
  name: name
  type: string
- description: Deal value/amount
  name: amount
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Current pipeline stage
  name: stage
  type: string
- description: Win probability percentage
  name: probability
  type: number
- description: Expected or actual close date
  name: closeDate
  type: string
- description: Deal owner user ID
  name: ownerId
  type: string
- description: Associated contact ID
  name: contactId
  type: string
- description: Associated company ID
  name: companyId
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: Non-unified fields from the source CRM provider
  name: additional
  type: object
provider_name: Revert
provider_slug: revert
schema_file: json-schema/revert-deal-schema.json
slug: revert-deal
source_filename: revert-deal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/revert/main/json-schema/revert-deal-schema.json\",\n  \"title\": \"Revert Unified CRM Deal\",\n  \"description\": \"Normalized deal/opportunity entity returned by the Revert Unified CRM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Revert-normalized unique deal identifier\"\n    },\n    \"remoteId\": {\n      \"type\": \"string\",\n      \"description\": \"The original ID from the source CRM provider\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Deal name or title\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Deal value/amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\"\n    },\n    \"stage\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Current pipeline stage\"\n    },\n    \"probability\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Win probability percentage\"\n    },\n    \"closeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expected or actual close date\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"Deal owner user ID\"\n    },\n    \"contactId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated contact ID\"\n    },\n    \"companyId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company ID\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"additional\": {\n      \"type\": \"object\",\n      \"description\": \"Non-unified fields from the source CRM provider\"\n    }\n\
  \  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/json-schema/revert-deal-schema.json
tags:
- Integrations
- CRM
- Unified API
- Open Source
title: Revert Unified CRM Deal
---
