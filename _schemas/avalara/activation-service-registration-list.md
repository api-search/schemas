---
description: RegistrationList schema from Avalara API
layout: schema
name: RegistrationList
properties_list:
- description: ''
  name: '@recordSetCount'
  type: integer
- description: ''
  name: value
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/activation-service-registration-list-schema.json
slug: activation-service-registration-list
source_filename: activation-service-registration-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/activation-service-registration-list-schema.json\",\n  \"title\": \"RegistrationList\",\n  \"description\": \"RegistrationList schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@recordSetCount\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Registration\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/activation-service-registration-list-schema.json
tags:
- Taxes
title: RegistrationList
---
