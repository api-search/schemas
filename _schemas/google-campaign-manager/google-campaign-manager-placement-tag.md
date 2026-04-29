---
description: A generated placement tag.
layout: schema
name: PlacementTag
properties_list:
- description: The placement ID this tag is generated for.
  name: placementId
  type: string
- description: Tags generated for this placement.
  name: tagDatas
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-placement-tag-schema.json
slug: google-campaign-manager-placement-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlacementTag\",\n  \"type\": \"object\",\n  \"description\": \"A generated placement tag.\",\n  \"properties\": {\n    \"placementId\": {\n      \"type\": \"string\",\n      \"description\": \"The placement ID this tag is generated for.\"\n    },\n    \"tagDatas\": {\n      \"type\": \"array\",\n      \"description\": \"Tags generated for this placement.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-placement-tag-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: PlacementTag
---
