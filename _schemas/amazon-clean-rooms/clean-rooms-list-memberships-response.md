---
description: Response for listing memberships.
layout: schema
name: ListMembershipsResponse
properties_list:
- description: The token value retrieved from a previous paginated request.
  name: nextToken
  type: string
- description: The list of memberships.
  name: membershipList
  type: array
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-list-memberships-response-schema.json
slug: clean-rooms-list-memberships-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-memberships-response-schema.json\",\n  \"title\": \"ListMembershipsResponse\",\n  \"description\": \"Response for listing memberships.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token value retrieved from a previous paginated request.\"\n    },\n    \"membershipList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Membership\"\n      },\n      \"description\": \"The list of memberships.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-memberships-response-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: ListMembershipsResponse
---
