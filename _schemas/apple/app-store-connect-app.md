---
description: ''
layout: schema
name: App
properties_list:
- description: ''
  name: type
  type: string
- description: The opaque resource ID that uniquely identifies the app
  name: id
  type: string
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-app-schema.json
slug: app-store-connect-app
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"App\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The opaque resource ID that uniquely identifies the app\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-app-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: App
---
