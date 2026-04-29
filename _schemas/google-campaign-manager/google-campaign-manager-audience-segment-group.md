---
description: Audience segment group for targeting.
layout: schema
name: AudienceSegmentGroup
properties_list:
- description: ID of this audience segment group.
  name: id
  type: string
- description: Name of this audience segment group.
  name: name
  type: string
- description: Audience segments assigned to this group.
  name: audienceSegments
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-audience-segment-group-schema.json
slug: google-campaign-manager-audience-segment-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AudienceSegmentGroup\",\n  \"type\": \"object\",\n  \"description\": \"Audience segment group for targeting.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of this audience segment group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of this audience segment group.\"\n    },\n    \"audienceSegments\": {\n      \"type\": \"array\",\n      \"description\": \"Audience segments assigned to this group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-audience-segment-group-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: AudienceSegmentGroup
---
