---
description: PaginationLinks schema from Adyen API
layout: schema
name: PaginationLinks
properties_list:
- description: The first page.
  name: first
  type: object
- description: The last page.
  name: last
  type: object
- description: The next page. Only present if there is a next page.
  name: next
  type: object
- description: The previous page. Only present if there is a previous page.
  name: prev
  type: object
- description: The current page.
  name: self
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-pagination-links-schema.json
slug: management-pagination-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-pagination-links-schema.json\",\n  \"title\": \"PaginationLinks\",\n  \"description\": \"PaginationLinks schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first\": {\n      \"description\": \"The first page.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"last\": {\n      \"description\": \"The last page.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"next\": {\n      \"description\": \"The next page. Only present if there is a next page.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"prev\": {\n      \"description\": \"The previous page. Only present if there is a previous page.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"self\": {\n      \"description\": \"The current\
  \ page.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    }\n  },\n  \"required\": [\n    \"self\",\n    \"first\",\n    \"last\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-pagination-links-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaginationLinks
---
