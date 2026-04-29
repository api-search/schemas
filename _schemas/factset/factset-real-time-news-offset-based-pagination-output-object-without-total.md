---
description: Pagination attributes for the offset-based pagination strategy; a total element count is not supported.
layout: schema
name: OffsetBasedPaginationOutputObjectWithoutTotal
properties_list:
- description: Flag indicating that a subsequent request with the same parameters, except that the parameter `pagination.offset` is incremented by `pagination.limit`, would yield additional results.
  name: hasNext
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-real-time-news-offset-based-pagination-output-object-without-total-schema.json
slug: factset-real-time-news-offset-based-pagination-output-object-without-total
source_filename: factset-real-time-news-offset-based-pagination-output-object-without-total-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OffsetBasedPaginationOutputObjectWithoutTotal\",\n  \"type\": \"object\",\n  \"description\": \"Pagination attributes for the offset-based pagination strategy; a total element count is not supported.\",\n  \"properties\": {\n    \"hasNext\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating that a subsequent request with the same parameters, except that the parameter `pagination.offset` is incremented by `pagination.limit`, would yield additional results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-real-time-news-offset-based-pagination-output-object-without-total-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: OffsetBasedPaginationOutputObjectWithoutTotal
---
