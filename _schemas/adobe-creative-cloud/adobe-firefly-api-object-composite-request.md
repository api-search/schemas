---
description: ObjectCompositeRequest from Adobe API
layout: schema
name: ObjectCompositeRequest
properties_list:
- description: ''
  name: image
  type: object
- description: Placement configuration for the object.
  name: placement
  type: object
- description: Optional text to guide the composition.
  name: prompt
  type: string
- description: ''
  name: numVariations
  type: integer
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-object-composite-request-schema.json
slug: adobe-firefly-api-object-composite-request
source_filename: adobe-firefly-api-object-composite-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-object-composite-request-schema.json\",\n  \"title\": \"ObjectCompositeRequest\",\n  \"description\": \"ObjectCompositeRequest from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"$ref\": \"#/components/schemas/ImageReference\"\n    },\n    \"placement\": {\n      \"type\": \"object\",\n      \"description\": \"Placement configuration for the object.\",\n      \"properties\": {\n        \"inpaint\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to harmonize the placed object.\"\n        }\n      }\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Optional text to guide the composition.\",\n      \"example\": \"A beautiful sunset over the ocean\"\n    },\n    \"numVariations\": {\n  \
  \    \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"example\": 42\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"placement\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-object-composite-request-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: ObjectCompositeRequest
---
