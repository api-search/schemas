---
description: TenantList schema from ARGUS Enterprise API
layout: schema
name: TenantList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-tenant-list-schema.json
slug: argus-enterprise-tenant-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-tenant-list-schema.json\",\n  \"title\": \"TenantList\",\n  \"description\": \"TenantList schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tenant\"\n      }\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/Pagination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-tenant-list-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: TenantList
---
