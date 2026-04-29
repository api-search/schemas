---
description: Video settings for in-stream video placements.
layout: schema
name: VideoSettings
properties_list:
- description: Companion ad settings.
  name: companionSettings
  type: object
- description: Transcode settings.
  name: transcodeSettings
  type: object
- description: Skippability settings.
  name: skippableSettings
  type: object
- description: Whether OBA icons are enabled for this placement.
  name: obaEnabled
  type: boolean
- description: ''
  name: obaSettings
  type: object
- description: Video orientation setting.
  name: orientation
  type: string
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-video-settings-schema.json
slug: google-campaign-manager-video-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoSettings\",\n  \"type\": \"object\",\n  \"description\": \"Video settings for in-stream video placements.\",\n  \"properties\": {\n    \"companionSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Companion ad settings.\"\n    },\n    \"transcodeSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Transcode settings.\"\n    },\n    \"skippableSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Skippability settings.\"\n    },\n    \"obaEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether OBA icons are enabled for this placement.\"\n    },\n    \"obaSettings\": {\n      \"type\": \"object\"\n    },\n    \"orientation\": {\n      \"type\": \"string\",\n      \"description\": \"Video orientation setting.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-video-settings-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: VideoSettings
---
