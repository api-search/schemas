---
description: Represents a teardown tag relationship. A teardown tag fires after the main tag.
layout: schema
name: TeardownTag
properties_list:
- description: The name of the teardown tag.
  name: tagName
  type: string
- description: If true, fire the teardown tag if and only if the main tag fires successfully. If false, fire the teardown tag regardless of main tag firing status.
  name: stopTeardownOnFailure
  type: boolean
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-teardown-tag-schema.json
slug: google-tag-manager-v2-teardown-tag
source_filename: google-tag-manager-v2-teardown-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TeardownTag\",\n  \"type\": \"object\",\n  \"description\": \"Represents a teardown tag relationship. A teardown tag fires after the main tag.\",\n  \"properties\": {\n    \"tagName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the teardown tag.\"\n    },\n    \"stopTeardownOnFailure\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, fire the teardown tag if and only if the main tag fires successfully. If false, fire the teardown tag regardless of main tag firing status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-teardown-tag-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: TeardownTag
---
