---
description: Response containing the record count for a query.
layout: schema
name: Count Response
properties_list:
- description: Total number of records matching the query parameters.
  name: count
  type: integer
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
schema_file: json-schema/quickstats-api-count-response-schema.json
slug: quickstats-api-count-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-count-response-schema.json\",\n  \"title\": \"Count Response\",\n  \"description\": \"Response containing the record count for a query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records matching the query parameters.\",\n      \"example\": 1250\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-count-response-schema.json
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
title: Count Response
---
