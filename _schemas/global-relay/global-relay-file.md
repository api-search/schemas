---
description: A file attachment uploaded to the Global Relay Archive, referenced by conversations, emails, voice records, or event cards.
layout: schema
name: Global Relay File
properties_list:
- description: Unique identifier for the file
  name: fileId
  type: string
- description: Original filename
  name: fileName
  type: string
- description: MIME type of the file
  name: contentType
  type: string
- description: Status of the file upload
  name: status
  type: string
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-file.json
slug: global-relay-file
source_filename: global-relay-file.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-file.json\",\n  \"title\": \"Global Relay File\",\n  \"description\": \"A file attachment uploaded to the Global Relay Archive, referenced by conversations, emails, voice records, or event cards.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"fileId\"\n  ],\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the file\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"Original filename\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the file\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the file upload\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-file.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay File
---
