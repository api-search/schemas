---
description: Custom rich media events for report filtering.
layout: schema
name: CustomRichMediaEvents
properties_list:
- description: List of custom rich media event IDs.
  name: filteredEventIds
  type: array
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-custom-rich-media-events-schema.json
slug: google-campaign-manager-custom-rich-media-events
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomRichMediaEvents\",\n  \"type\": \"object\",\n  \"description\": \"Custom rich media events for report filtering.\",\n  \"properties\": {\n    \"filteredEventIds\": {\n      \"type\": \"array\",\n      \"description\": \"List of custom rich media event IDs.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-custom-rich-media-events-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: CustomRichMediaEvents
---
