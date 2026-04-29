---
description: error schema from Acquia Cloud API
layout: schema
name: Error
properties_list:
- description: The error summary.
  name: error
  type: string
- description: The long description for the returned error.
  name: message
  type: string
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-error-schema.json
slug: acquia-cloud-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"error schema from Acquia Cloud API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"The error summary.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The long description for the returned error.\"\n    }\n  },\n  \"required\": [\n    \"error\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-error-schema.json
tags:
- Content
- Experience
title: Error
---
