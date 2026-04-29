---
description: Tenant schema from ARGUS Enterprise API
layout: schema
name: Tenant
properties_list:
- description: Unique tenant identifier
  name: id
  type: string
- description: Tenant company or individual name
  name: name
  type: string
- description: Tenant industry classification
  name: industry
  type: string
- description: Tenant credit rating
  name: creditRating
  type: string
- description: Primary contact name
  name: contactName
  type: string
- description: Primary contact email
  name: contactEmail
  type: string
- description: Primary contact phone
  name: contactPhone
  type: string
- description: ''
  name: address
  type: object
- description: Number of active leases
  name: activeLeases
  type: integer
- description: Total leased area across all properties
  name: totalLeasedArea
  type: number
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-tenant-schema.json
slug: argus-enterprise-tenant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-tenant-schema.json\",\n  \"title\": \"Tenant\",\n  \"description\": \"Tenant schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique tenant identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant company or individual name\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant industry classification\"\n    },\n    \"creditRating\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant credit rating\"\n    },\n    \"contactName\": {\n      \"type\": \"string\",\n      \"description\": \"Primary contact name\"\n    },\n    \"contactEmail\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"email\",\n      \"description\": \"Primary contact email\"\n    },\n    \"contactPhone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary contact phone\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"activeLeases\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active leases\"\n    },\n    \"totalLeasedArea\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total leased area across all properties\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-tenant-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Tenant
---
