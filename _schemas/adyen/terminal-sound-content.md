---
description: SoundContent schema from Adyen API
layout: schema
name: SoundContent
properties_list:
- description: ''
  name: SoundFormat
  type: object
- description: ''
  name: Language
  type: string
- description: ''
  name: ReferenceID
  type: string
- description: ''
  name: Text
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sound-content-schema.json
slug: terminal-sound-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sound-content-schema.json\",\n  \"title\": \"SoundContent\",\n  \"description\": \"SoundContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SoundFormat\": {\n      \"$ref\": \"#/components/schemas/SoundFormat\"\n    },\n    \"Language\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\"\n    },\n    \"ReferenceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"Text\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"SoundFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sound-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SoundContent
---
