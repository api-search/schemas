---
description: Pagination attributes for the offset-based pagination strategy.
layout: schema
name: OffsetBasedPaginationOutputObject
properties_list:
- description: Total number of entries in the result set.
  name: total
  type: number
- description: Flag indicating that the value of "total" is estimated.
  name: isEstimatedTotal
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-securitized-derivatives-for-digital-portals-offset-based-pagination-output-object-schema.json
slug: factset-securitized-derivatives-for-digital-portals-offset-based-pagination-output-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OffsetBasedPaginationOutputObject\",\n  \"type\": \"object\",\n  \"description\": \"Pagination attributes for the offset-based pagination strategy.\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of entries in the result set.\"\n    },\n    \"isEstimatedTotal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating that the value of \\\"total\\\" is estimated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-securitized-derivatives-for-digital-portals-offset-based-pagination-output-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: OffsetBasedPaginationOutputObject
---
