---
description: A paginated list of group resources.
layout: schema
name: Groups
properties_list:
- description: The type of the API resource.
  name: kind
  type: string
- description: ETag of the resource.
  name: etag
  type: string
- description: A list of group objects.
  name: groups
  type: array
- description: Token for retrieving the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Workspace
provider_slug: google-workspace
schema_file: json-schema/admin-sdk-directory-groups-schema.json
slug: admin-sdk-directory-groups
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Groups\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of group resources.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the API resource.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag of the resource.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"A list of group objects.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for retrieving the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/json-schema/admin-sdk-directory-groups-schema.json
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
title: Groups
---
