---
description: Schema for a Rainbow CPaaS contact / user profile
layout: schema
name: Rainbow Contact
properties_list:
- description: Unique contact identifier
  name: id
  type: string
- description: Contact's display name
  name: displayName
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: emails
  type: array
- description: ''
  name: phoneNumbers
  type: array
- description: ''
  name: presence
  type: object
- description: ''
  name: company
  type: string
- description: ''
  name: jobTitle
  type: string
provider_name: Rainbow
provider_slug: rainbow
schema_file: json-schema/rainbow-contact-schema.json
slug: rainbow-contact
source_filename: rainbow-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://openrainbow.com/schemas/contact\",\n  \"title\": \"Rainbow Contact\",\n  \"description\": \"Schema for a Rainbow CPaaS contact / user profile\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"displayName\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique contact identifier\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Contact's display name\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": { \"type\": \"string\", \"format\": \"email\" },\n          \"type\": { \"type\": \"string\", \"enum\": [\"work\", \"personal\", \"other\"] }\n        }\n      }\n    },\n    \"phoneNumbers\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\", \"enum\": [\"work\", \"mobile\", \"home\", \"other\"] }\n        }\n      }\n    },\n    \"presence\": {\n      \"$ref\": \"#/$defs/Presence\"\n    },\n    \"company\": {\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$defs\": {\n    \"Presence\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"online\", \"away\", \"busy\", \"dnd\", \"offline\"]\n        },\n        \"statusMessage\": { \"type\": \"string\" },\n        \"since\": { \"type\": \"string\", \"format\": \"date-time\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/json-schema/rainbow-contact-schema.json
tags:
- Communications
- CPaaS
- Chat
- Voice
- Video
- Telephony
- Messaging
- Collaboration
- Unified Communications
title: Rainbow Contact
---
