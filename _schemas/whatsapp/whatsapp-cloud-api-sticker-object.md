---
description: StickerObject from WhatsApp API
layout: schema
name: StickerObject
properties_list:
- description: Media ID from upload
  name: id
  type: string
- description: HTTPS URL of the sticker (WebP format)
  name: link
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-sticker-object-schema.json
slug: whatsapp-cloud-api-sticker-object
source_filename: whatsapp-cloud-api-sticker-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-sticker-object-schema.json\",\n  \"title\": \"StickerObject\",\n  \"description\": \"StickerObject from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Media ID from upload\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS URL of the sticker (WebP format)\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-sticker-object-schema.json
tags: []
title: StickerObject
---
