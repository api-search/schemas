---
description: Pagination attributes for the cursor-based pagination strategy; a total element count is not supported.
layout: schema
name: CursorBasedPaginationOutputObjectWithoutTotal
properties_list:
- description: The next cursor position to use in the parameter `pagination.cursor` for an endpoint that supports cursor-based pagination, otherwise `null`.
  name: next
  type: string
- description: 'The previous cursor position to use in the parameter `pagination.cursor` for an endpoint that supports cursor-based pagination. If a previous cursor position is not supported or available, `previous` '
  name: previous
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-securitized-derivatives-for-digital-portals-cursor-based-pagination-output-object-without-total-schema.json
slug: factset-securitized-derivatives-for-digital-portals-cursor-based-pagination-output-object-without-total
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CursorBasedPaginationOutputObjectWithoutTotal\",\n  \"type\": \"object\",\n  \"description\": \"Pagination attributes for the cursor-based pagination strategy; a total element count is not supported.\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"The next cursor position to use in the parameter `pagination.cursor` for an endpoint that supports cursor-based pagination, otherwise `null`.\"\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"description\": \"The previous cursor position to use in the parameter `pagination.cursor` for an endpoint that supports cursor-based pagination. If a previous cursor position is not supported or available, `previous` is `null`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-securitized-derivatives-for-digital-portals-cursor-based-pagination-output-object-without-total-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CursorBasedPaginationOutputObjectWithoutTotal
---
