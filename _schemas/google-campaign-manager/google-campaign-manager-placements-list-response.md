---
description: Placement list response.
layout: schema
name: PlacementsListResponse
properties_list:
- description: ''
  name: placements
  type: array
- description: ''
  name: nextPageToken
  type: string
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-placements-list-response-schema.json
slug: google-campaign-manager-placements-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlacementsListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Placement list response.\",\n  \"properties\": {\n    \"placements\": {\n      \"type\": \"array\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-placements-list-response-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: PlacementsListResponse
---
