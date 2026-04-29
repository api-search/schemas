---
description: An embedded object such as an image.
layout: schema
name: EmbeddedObject
properties_list:
- description: The title of the embedded object.
  name: title
  type: string
- description: The description of the embedded object.
  name: description
  type: string
- description: Properties of an embedded drawing. Currently empty.
  name: embeddedDrawingProperties
  type: object
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-embedded-object-schema.json
slug: google-docs-v1-embedded-object
source_filename: google-docs-v1-embedded-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddedObject\",\n  \"type\": \"object\",\n  \"description\": \"An embedded object such as an image.\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the embedded object.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the embedded object.\"\n    },\n    \"embeddedDrawingProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties of an embedded drawing. Currently empty.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-embedded-object-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: EmbeddedObject
---
