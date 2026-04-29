---
description: Represents a file uploaded to Affirm's servers.
layout: schema
name: FileObject
properties_list:
- description: Unique identifier for the uploaded file.
  name: id
  type: string
- description: Original filename of the uploaded file.
  name: filename
  type: string
- description: File size in bytes.
  name: size
  type: integer
- description: MIME type of the uploaded file.
  name: content_type
  type: string
- description: Intended purpose of the file.
  name: purpose
  type: string
- description: Upload timestamp in RFC 3339 format.
  name: created
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/direct-api-file-object-schema.json
slug: direct-api-file-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/direct-api-file-object-schema.json\",\n  \"title\": \"FileObject\",\n  \"description\": \"Represents a file uploaded to Affirm's servers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the uploaded file.\",\n      \"example\": \"500123\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Original filename of the uploaded file.\",\n      \"example\": \"Example Merchant\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes.\",\n      \"example\": 1\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the uploaded file.\",\n      \"example\": \"standard\"\n    },\n    \"purpose\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Intended purpose of the file.\",\n      \"example\": \"example_value\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Upload timestamp in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/direct-api-file-object-schema.json
tags: []
title: FileObject
---
