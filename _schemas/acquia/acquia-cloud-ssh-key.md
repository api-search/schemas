---
description: Details an SSH key.
layout: schema
name: Ssh Key
properties_list:
- description: The unique identifier of the SSH key.
  name: uuid
  type: string
- description: The human-readable key label.
  name: label
  type: string
- description: The public key.
  name: public_key
  type: string
- description: The public key fingerprint.
  name: fingerprint
  type: string
- description: The key creation date.
  name: created_at
  type: string
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-ssh-key-schema.json
slug: acquia-cloud-ssh-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-ssh-key-schema.json\",\n  \"title\": \"Ssh Key\",\n  \"description\": \"Details an SSH key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the SSH key.\",\n      \"format\": \"uuid\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable key label.\"\n    },\n    \"public_key\": {\n      \"type\": \"string\",\n      \"description\": \"The public key.\",\n      \"minLength\": 64\n    },\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"The public key fingerprint.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The key creation date.\"\n    },\n    \"_links\"\
  : {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"label\",\n    \"public_key\",\n    \"fingerprint\",\n    \"created_at\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-ssh-key-schema.json
tags:
- Content
- Experience
title: Ssh Key
---
