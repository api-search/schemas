---
description: Pagination metadata for list responses
layout: schema
name: PaginationInfo
properties_list:
- description: Number of records per page
  name: pageSize
  type: integer
- description: Current page offset
  name: pageStart
  type: integer
- description: Total number of records available
  name: totalRecords
  type: integer
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-pagination-info-schema.json
slug: temenos-transact-core-banking-pagination-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationInfo\",\n  \"type\": \"object\",\n  \"description\": \"Pagination metadata for list responses\",\n  \"properties\": {\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records per page\"\n    },\n    \"pageStart\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page offset\"\n    },\n    \"totalRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records available\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-pagination-info-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: PaginationInfo
---
