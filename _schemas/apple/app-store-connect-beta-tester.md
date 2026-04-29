---
description: ''
layout: schema
name: BetaTester
properties_list:
- description: ''
  name: type
  type: string
- description: The opaque resource ID that uniquely identifies the beta tester
  name: id
  type: string
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-beta-tester-schema.json
slug: app-store-connect-beta-tester
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BetaTester\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The opaque resource ID that uniquely identifies the beta tester\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-beta-tester-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: BetaTester
---
