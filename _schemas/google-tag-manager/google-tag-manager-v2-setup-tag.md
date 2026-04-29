---
description: Represents a setup tag relationship. A setup tag fires before the main tag.
layout: schema
name: SetupTag
properties_list:
- description: The name of the setup tag.
  name: tagName
  type: string
- description: If true, fire the main tag only if the setup tag fires successfully. If false, fire the main tag regardless of setup tag firing status.
  name: stopOnSetupFailure
  type: boolean
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-setup-tag-schema.json
slug: google-tag-manager-v2-setup-tag
source_filename: google-tag-manager-v2-setup-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SetupTag\",\n  \"type\": \"object\",\n  \"description\": \"Represents a setup tag relationship. A setup tag fires before the main tag.\",\n  \"properties\": {\n    \"tagName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the setup tag.\"\n    },\n    \"stopOnSetupFailure\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, fire the main tag only if the setup tag fires successfully. If false, fire the main tag regardless of setup tag firing status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-setup-tag-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: SetupTag
---
