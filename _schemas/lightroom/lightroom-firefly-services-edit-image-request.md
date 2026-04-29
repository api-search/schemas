---
description: ''
layout: schema
name: EditImageRequest
properties_list:
- description: ''
  name: inputs
  type: object
- description: ''
  name: outputs
  type: array
- description: Lightroom develop settings to apply. All values are optional and correspond to Lightroom develop module parameters.
  name: options
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-firefly-services-edit-image-request-schema.json
slug: lightroom-firefly-services-edit-image-request
source_filename: lightroom-firefly-services-edit-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EditImageRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"object\"\n    },\n    \"outputs\": {\n      \"type\": \"array\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Lightroom develop settings to apply. All values are optional and correspond to Lightroom develop module parameters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-firefly-services-edit-image-request-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: EditImageRequest
---
