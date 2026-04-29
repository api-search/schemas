---
description: A request to compose objects.
layout: schema
name: ComposeRequest
properties_list:
- description: The kind of item this is.
  name: kind
  type: string
- description: The list of source objects that will be concatenated into a single object. Maximum 32 objects.
  name: sourceObjects
  type: array
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
schema_file: json-schema/gcp-cloud-storage-json-compose-request-schema.json
slug: gcp-cloud-storage-json-compose-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComposeRequest\",\n  \"type\": \"object\",\n  \"description\": \"A request to compose objects.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of item this is.\"\n    },\n    \"sourceObjects\": {\n      \"type\": \"array\",\n      \"description\": \"The list of source objects that will be concatenated into a single object. Maximum 32 objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/json-schema/gcp-cloud-storage-json-compose-request-schema.json
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
title: ComposeRequest
---
