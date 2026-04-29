---
description: ''
layout: schema
name: GrammarFile
properties_list:
- description: ''
  name: fileName
  type: string
- description: ''
  name: filePath
  type: string
- description: ''
  name: fileType
  type: string
- description: ''
  name: fileSize
  type: integer
- description: Language of the grammar (e.g., en-US)
  name: language
  type: string
- description: ''
  name: lastModified
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-grammar-file-schema.json
slug: cisco-voice-portal-vxml-services-grammar-file
source_filename: cisco-voice-portal-vxml-services-grammar-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GrammarFile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\"\n    },\n    \"filePath\": {\n      \"type\": \"string\"\n    },\n    \"fileType\": {\n      \"type\": \"string\"\n    },\n    \"fileSize\": {\n      \"type\": \"integer\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the grammar (e.g., en-US)\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-grammar-file-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: GrammarFile
---
