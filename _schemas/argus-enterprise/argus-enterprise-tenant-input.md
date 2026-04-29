---
description: TenantInput schema from ARGUS Enterprise API
layout: schema
name: TenantInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: industry
  type: string
- description: ''
  name: creditRating
  type: string
- description: ''
  name: contactName
  type: string
- description: ''
  name: contactEmail
  type: string
- description: ''
  name: contactPhone
  type: string
- description: ''
  name: address
  type: object
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-tenant-input-schema.json
slug: argus-enterprise-tenant-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-tenant-input-schema.json\",\n  \"title\": \"TenantInput\",\n  \"description\": \"TenantInput schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"industry\": {\n      \"type\": \"string\"\n    },\n    \"creditRating\": {\n      \"type\": \"string\"\n    },\n    \"contactName\": {\n      \"type\": \"string\"\n    },\n    \"contactEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"contactPhone\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-tenant-input-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: TenantInput
---
