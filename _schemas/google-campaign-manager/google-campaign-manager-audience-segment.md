---
description: An audience segment for targeting.
layout: schema
name: AudienceSegment
properties_list:
- description: ID of this audience segment.
  name: id
  type: string
- description: Name of this audience segment.
  name: name
  type: string
- description: Weight allocated to this segment. Must be between 1 and 1000.
  name: allocation
  type: integer
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-audience-segment-schema.json
slug: google-campaign-manager-audience-segment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AudienceSegment\",\n  \"type\": \"object\",\n  \"description\": \"An audience segment for targeting.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of this audience segment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of this audience segment.\"\n    },\n    \"allocation\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight allocated to this segment. Must be between 1 and 1000.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-audience-segment-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: AudienceSegment
---
