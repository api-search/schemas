---
description: The properties of a Page that are only relevant for pages with pageType MASTER.
layout: schema
name: MasterProperties
properties_list:
- description: The human-readable name of the master.
  name: displayName
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-master-properties-schema.json
slug: google-slides-master-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MasterProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a Page that are only relevant for pages with pageType MASTER.\\n\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the master.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-master-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: MasterProperties
---
