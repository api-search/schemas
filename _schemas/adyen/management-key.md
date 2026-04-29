---
description: Key schema from Adyen API
layout: schema
name: Key
properties_list:
- description: The unique identifier of the shared key.
  name: identifier
  type: string
- description: The secure passphrase to protect the shared key.
  name: passphrase
  type: string
- description: The version number of the shared key.
  name: version
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-key-schema.json
slug: management-key
source_filename: management-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-key-schema.json\",\n  \"title\": \"Key\",\n  \"description\": \"Key schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"description\": \"The unique identifier of the shared key.\",\n      \"type\": \"string\"\n    },\n    \"passphrase\": {\n      \"description\": \"The secure passphrase to protect the shared key.\",\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"description\": \"The version number of the shared key.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-key-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Key
---
