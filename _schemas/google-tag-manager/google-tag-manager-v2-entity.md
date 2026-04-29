---
description: A workspace entity that can represent a tag, trigger, variable, or folder that has been changed.
layout: schema
name: Entity
properties_list:
- description: The status of the entity change.
  name: changeStatus
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-entity-schema.json
slug: google-tag-manager-v2-entity
source_filename: google-tag-manager-v2-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Entity\",\n  \"type\": \"object\",\n  \"description\": \"A workspace entity that can represent a tag, trigger, variable, or folder that has been changed.\",\n  \"properties\": {\n    \"changeStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the entity change.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-entity-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: Entity
---
