---
description: A sorted dimension for report queries.
layout: schema
name: SortedDimension
properties_list:
- description: The name of the dimension.
  name: name
  type: string
- description: The sort order of this dimension.
  name: sortOrder
  type: string
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-sorted-dimension-schema.json
slug: google-campaign-manager-sorted-dimension
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SortedDimension\",\n  \"type\": \"object\",\n  \"description\": \"A sorted dimension for report queries.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dimension.\"\n    },\n    \"sortOrder\": {\n      \"type\": \"string\",\n      \"description\": \"The sort order of this dimension.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-sorted-dimension-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: SortedDimension
---
