---
description: Tag settings for a placement.
layout: schema
name: TagSetting
properties_list:
- description: Additional key-values to append to tags.
  name: additionalKeyValues
  type: string
- description: Whether to include click-tracking string in tags.
  name: includeClickTracking
  type: boolean
- description: Whether to include click-through URLs in tags.
  name: includeClickThroughUrls
  type: boolean
- description: Option specifying how keywords are embedded in ad tags.
  name: keywordOption
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-tag-setting-schema.json
slug: google-campaign-manager-tag-setting
source_filename: google-campaign-manager-tag-setting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagSetting\",\n  \"type\": \"object\",\n  \"description\": \"Tag settings for a placement.\",\n  \"properties\": {\n    \"additionalKeyValues\": {\n      \"type\": \"string\",\n      \"description\": \"Additional key-values to append to tags.\"\n    },\n    \"includeClickTracking\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include click-tracking string in tags.\"\n    },\n    \"includeClickThroughUrls\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include click-through URLs in tags.\"\n    },\n    \"keywordOption\": {\n      \"type\": \"string\",\n      \"description\": \"Option specifying how keywords are embedded in ad tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-tag-setting-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: TagSetting
---
