---
description: ''
layout: schema
name: ApiKey
properties_list:
- description: API key creation date in ISO 8601 format
  name: date
  type: string
- description: A free-text human readable description of this API key
  name: description
  type: string
- description: API key expiration date in ISO 8601 format
  name: expirationDate
  type: string
- description: API Key identifier
  name: id
  type: string
- description: The API Key secret to be used to retrieve acces tokens. This field is only provided once, then the client should store this information in a secure place.
  name: secret
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-api-key-schema.json
slug: oneatlas-api-key
source_filename: oneatlas-api-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-api-key-schema.json\",\n  \"title\": \"ApiKey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"description\": \"API key creation date in ISO 8601 format\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"A free-text human readable description of this API key\",\n      \"type\": \"string\"\n    },\n    \"expirationDate\": {\n      \"description\": \"API key expiration date in ISO 8601 format\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"API Key identifier\",\n      \"type\": \"string\"\n    },\n    \"secret\": {\n      \"description\": \"The API Key secret to be used to retrieve acces tokens. This field is only provided once, then the client should store this information in a secure place.\",\n   \
  \   \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"description\",\n    \"date\",\n    \"expirationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-api-key-schema.json
tags:
- Imagery
- Satellites
title: ApiKey
---
