---
description: ''
layout: schema
name: Build
properties_list:
- description: ''
  name: type
  type: string
- description: The opaque resource ID that uniquely identifies the build
  name: id
  type: string
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-build-schema.json
slug: app-store-connect-build
source_filename: app-store-connect-build-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Build\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The opaque resource ID that uniquely identifies the build\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-build-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: Build
---
