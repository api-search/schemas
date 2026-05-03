---
description: A Credential represents a Connected User's authentication tokens for a specific third-party integration.
layout: schema
name: Paragon Credential
properties_list:
- description: The unique identifier for the credential.
  name: id
  type: string
- description: The integration this credential belongs to.
  name: integrationId
  type: string
- description: The current status of the credential.
  name: status
  type: string
provider_name: Paragon
provider_slug: paragon
schema_file: json-schema/credential.json
slug: credential
source_filename: credential.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/paragon/blob/main/json-schema/credential.json\",\n  \"title\": \"Paragon Credential\",\n  \"description\": \"A Credential represents a Connected User's authentication tokens for a specific third-party integration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the credential.\"\n    },\n    \"integrationId\": {\n      \"type\": \"string\",\n      \"description\": \"The integration this credential belongs to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the credential.\",\n      \"enum\": [\"VALID\", \"INVALID\", \"EXPIRED\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/json-schema/credential.json
tags:
- Embedded iPaaS
- Integrations
title: Paragon Credential
---
