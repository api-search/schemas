---
description: ListTerminalsResponse schema from Adyen API
layout: schema
name: ListTerminalsResponse
properties_list:
- description: Pagination references.
  name: _links
  type: object
- description: The list of terminals and their details.
  name: data
  type: array
- description: Total number of items.
  name: itemsTotal
  type: integer
- description: Total number of pages.
  name: pagesTotal
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-list-terminals-response-schema.json
slug: management-list-terminals-response
source_filename: management-list-terminals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-list-terminals-response-schema.json\",\n  \"title\": \"ListTerminalsResponse\",\n  \"description\": \"ListTerminalsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"Pagination references.\",\n      \"$ref\": \"#/components/schemas/PaginationLinks\"\n    },\n    \"data\": {\n      \"description\": \"The list of terminals and their details.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Terminal\"\n      },\n      \"type\": \"array\"\n    },\n    \"itemsTotal\": {\n      \"description\": \"Total number of items.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"pagesTotal\": {\n      \"description\": \"Total number of pages.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\
  \n    }\n  },\n  \"required\": [\n    \"itemsTotal\",\n    \"pagesTotal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-list-terminals-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ListTerminalsResponse
---
