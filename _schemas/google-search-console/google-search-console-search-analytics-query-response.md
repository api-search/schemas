---
description: Response for a search analytics query.
layout: schema
name: SearchAnalyticsQueryResponse
properties_list:
- description: A list of rows grouped by the requested dimensions. Rows are ordered by click count descending. If no data is available for the specified date range and filters, this field is omitted.
  name: rows
  type: array
- description: How the results were aggregated.
  name: responseAggregationType
  type: string
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-search-analytics-query-response-schema.json
slug: google-search-console-search-analytics-query-response
source_filename: google-search-console-search-analytics-query-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchAnalyticsQueryResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response for a search analytics query.\",\n  \"properties\": {\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"A list of rows grouped by the requested dimensions. Rows are ordered by click count descending. If no data is available for the specified date range and filters, this field is omitted.\"\n    },\n    \"responseAggregationType\": {\n      \"type\": \"string\",\n      \"description\": \"How the results were aggregated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-search-analytics-query-response-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: SearchAnalyticsQueryResponse
---
