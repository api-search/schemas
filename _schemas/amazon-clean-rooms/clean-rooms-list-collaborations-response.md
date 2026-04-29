---
description: Response for listing collaborations.
layout: schema
name: ListCollaborationsResponse
properties_list:
- description: The token value retrieved from a previous paginated request.
  name: nextToken
  type: string
- description: The list of collaborations.
  name: collaborationList
  type: array
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-list-collaborations-response-schema.json
slug: clean-rooms-list-collaborations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-collaborations-response-schema.json\",\n  \"title\": \"ListCollaborationsResponse\",\n  \"description\": \"Response for listing collaborations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token value retrieved from a previous paginated request.\"\n    },\n    \"collaborationList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Collaboration\"\n      },\n      \"description\": \"The list of collaborations.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-collaborations-response-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: ListCollaborationsResponse
---
