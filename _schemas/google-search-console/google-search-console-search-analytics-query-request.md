---
description: Request body for querying search analytics data. Defines the date range, dimensions, filters, and aggregation type for the query.
layout: schema
name: SearchAnalyticsQueryRequest
properties_list:
- description: Start date of the requested date range, in YYYY-MM-DD format. Must be less than or equal to the end date. Data is available starting from the date the site was added to Search Console.
  name: startDate
  type: string
- description: End date of the requested date range, in YYYY-MM-DD format. Must be greater than or equal to the start date. There is a processing delay of approximately 2-3 days.
  name: endDate
  type: string
- description: Zero or more dimensions to group results by. Results are grouped in the order that dimensions are specified. Valid dimensions are date, query, page, country, device, and searchAppearance.
  name: dimensions
  type: array
- description: Filter results to the specified search type. Defaults to web.
  name: type
  type: string
- description: Zero or more groups of dimension filters. All filter groups are ANDed together. Within a group, filters are combined using the group type (AND by default).
  name: dimensionFilterGroups
  type: array
- description: How data is aggregated. If auto, data is aggregated by property type. If byPage, all data is aggregated by page. If byProperty, all data is aggregated by property.
  name: aggregationType
  type: string
- description: Maximum number of rows to return. Valid range is 1 to 25000. Default is 1000.
  name: rowLimit
  type: integer
- description: Zero-based index of the first row in the response. Must be a non-negative number. Default is 0.
  name: startRow
  type: integer
- description: The data state to filter on. If set to final, only finalized data is returned. If set to all, both finalized and fresh data are included.
  name: dataState
  type: string
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-search-analytics-query-request-schema.json
slug: google-search-console-search-analytics-query-request
source_filename: google-search-console-search-analytics-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchAnalyticsQueryRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for querying search analytics data. Defines the date range, dimensions, filters, and aggregation type for the query.\",\n  \"properties\": {\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Start date of the requested date range, in YYYY-MM-DD format. Must be less than or equal to the end date. Data is available starting from the date the site was added to Search Console.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"End date of the requested date range, in YYYY-MM-DD format. Must be greater than or equal to the start date. There is a processing delay of approximately 2-3 days.\"\n    },\n    \"dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"Zero or more dimensions to group results by. Results are grouped in the order\
  \ that dimensions are specified. Valid dimensions are date, query, page, country, device, and searchAppearance.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Filter results to the specified search type. Defaults to web.\"\n    },\n    \"dimensionFilterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Zero or more groups of dimension filters. All filter groups are ANDed together. Within a group, filters are combined using the group type (AND by default).\"\n    },\n    \"aggregationType\": {\n      \"type\": \"string\",\n      \"description\": \"How data is aggregated. If auto, data is aggregated by property type. If byPage, all data is aggregated by page. If byProperty, all data is aggregated by property.\"\n    },\n    \"rowLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of rows to return. Valid range is 1 to 25000. Default is 1000.\"\n    },\n    \"startRow\": {\n      \"type\": \"integer\",\n     \
  \ \"description\": \"Zero-based index of the first row in the response. Must be a non-negative number. Default is 0.\"\n    },\n    \"dataState\": {\n      \"type\": \"string\",\n      \"description\": \"The data state to filter on. If set to final, only finalized data is returned. If set to all, both finalized and fresh data are included.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-search-analytics-query-request-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: SearchAnalyticsQueryRequest
---
