---
description: Response for listing protected queries.
layout: schema
name: ListProtectedQueriesResponse
properties_list:
- description: The token value retrieved from a previous paginated request.
  name: nextToken
  type: string
- description: The list of protected queries.
  name: protectedQueries
  type: array
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-list-protected-queries-response-schema.json
slug: clean-rooms-list-protected-queries-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-protected-queries-response-schema.json\",\n  \"title\": \"ListProtectedQueriesResponse\",\n  \"description\": \"Response for listing protected queries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token value retrieved from a previous paginated request.\"\n    },\n    \"protectedQueries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ProtectedQuery\"\n      },\n      \"description\": \"The list of protected queries.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-protected-queries-response-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: ListProtectedQueriesResponse
---
