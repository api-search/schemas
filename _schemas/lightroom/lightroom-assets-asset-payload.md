---
description: ''
layout: schema
name: AssetPayload
properties_list:
- description: Date and time the photo was captured
  name: captureDate
  type: string
- description: ''
  name: userCreated
  type: string
- description: ''
  name: userUpdated
  type: string
- description: ''
  name: importSource
  type: object
- description: Develop settings snapshot
  name: develop
  type: object
- description: Embedded XMP metadata
  name: xmp
  type: object
- description: ''
  name: location
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-assets-asset-payload-schema.json
slug: lightroom-assets-asset-payload
source_filename: lightroom-assets-asset-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetPayload\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"captureDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the photo was captured\"\n    },\n    \"userCreated\": {\n      \"type\": \"string\"\n    },\n    \"userUpdated\": {\n      \"type\": \"string\"\n    },\n    \"importSource\": {\n      \"type\": \"object\"\n    },\n    \"develop\": {\n      \"type\": \"object\",\n      \"description\": \"Develop settings snapshot\"\n    },\n    \"xmp\": {\n      \"type\": \"object\",\n      \"description\": \"Embedded XMP metadata\"\n    },\n    \"location\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-assets-asset-payload-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AssetPayload
---
