---
description: DocumentObject from WhatsApp API
layout: schema
name: DocumentObject
properties_list:
- description: Media ID from upload
  name: id
  type: string
- description: HTTPS URL of the document
  name: link
  type: string
- description: Caption text
  name: caption
  type: string
- description: Filename to display to recipient
  name: filename
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-document-object-schema.json
slug: whatsapp-cloud-api-document-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-document-object-schema.json\",\n  \"title\": \"DocumentObject\",\n  \"description\": \"DocumentObject from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Media ID from upload\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS URL of the document\",\n      \"example\": \"example_value\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"Caption text\",\n      \"example\": \"example_value\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Filename to display to recipient\",\n      \"example\": \"Example Business\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-document-object-schema.json
tags: []
title: DocumentObject
---
