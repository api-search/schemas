---
description: MediaObject from WhatsApp API
layout: schema
name: MediaObject
properties_list:
- description: Media ID from upload
  name: id
  type: string
- description: HTTPS URL of the media file
  name: link
  type: string
- description: Caption text
  name: caption
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-media-object-schema.json
slug: whatsapp-cloud-api-media-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-media-object-schema.json\",\n  \"title\": \"MediaObject\",\n  \"description\": \"MediaObject from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Media ID from upload\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS URL of the media file\",\n      \"example\": \"example_value\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"Caption text\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-media-object-schema.json
tags: []
title: MediaObject
---
