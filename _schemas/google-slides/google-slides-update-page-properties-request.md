---
description: Updates the properties of a Page.
layout: schema
name: UpdatePagePropertiesRequest
properties_list:
- description: The object ID of the page the update is applied to.
  name: objectId
  type: string
- description: The fields that should be updated.
  name: fields
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-page-properties-request-schema.json
slug: google-slides-update-page-properties-request
source_filename: google-slides-update-page-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdatePagePropertiesRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the properties of a Page.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the page the update is applied to.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-page-properties-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdatePagePropertiesRequest
---
