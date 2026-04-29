---
description: LocationMessage from WhatsApp API
layout: schema
name: LocationMessage
properties_list:
- description: ''
  name: latitude
  type: number
- description: ''
  name: longitude
  type: number
- description: Location name
  name: name
  type: string
- description: Location address
  name: address
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-location-message-schema.json
slug: whatsapp-cloud-api-location-message
source_filename: whatsapp-cloud-api-location-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-location-message-schema.json\",\n  \"title\": \"LocationMessage\",\n  \"description\": \"LocationMessage from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latitude\": {\n      \"type\": \"number\",\n      \"minimum\": -90,\n      \"maximum\": 90,\n      \"example\": 42.5\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"minimum\": -180,\n      \"maximum\": 180,\n      \"example\": 42.5\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Location name\",\n      \"example\": \"Example Business\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Location address\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"latitude\",\n    \"longitude\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-location-message-schema.json
tags: []
title: LocationMessage
---
