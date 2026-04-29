---
description: Pagination schema from ARGUS Enterprise API
layout: schema
name: Pagination
properties_list:
- description: Current page number
  name: page
  type: integer
- description: Number of items per page
  name: pageSize
  type: integer
- description: Total number of items
  name: totalItems
  type: integer
- description: Total number of pages
  name: totalPages
  type: integer
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-pagination-schema.json
slug: argus-enterprise-pagination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-pagination-schema.json\",\n  \"title\": \"Pagination\",\n  \"description\": \"Pagination schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page\"\n    },\n    \"totalItems\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of items\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pages\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-pagination-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Pagination
---
