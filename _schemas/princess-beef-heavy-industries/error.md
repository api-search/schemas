---
description: An error response from the API, following the RFC 7807 Problem Details format.
layout: schema
name: pb33f Giftshop Error
properties_list:
- description: The URI of the error type.
  name: type
  type: string
- description: A short, human-readable summary of the problem type.
  name: title
  type: string
- description: The HTTP status code applicable to this problem.
  name: status
  type: integer
- description: A human-readable explanation specific to this occurrence of the problem.
  name: detail
  type: string
- description: A URI reference that identifies the specific occurrence of the problem.
  name: instance
  type: string
provider_name: Princess Beef Heavy Industries
provider_slug: princess-beef-heavy-industries
schema_file: json-schema/error.json
slug: error
source_filename: error.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/princess-beef-heavy-industries/blob/main/json-schema/error.json\",\n  \"title\": \"pb33f Giftshop Error\",\n  \"description\": \"An error response from the API, following the RFC 7807 Problem Details format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The URI of the error type.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"maxLength\": 200,\n      \"description\": \"A short, human-readable summary of the problem type.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"minimum\": 100,\n      \"maximum\": 500,\n      \"description\": \"The HTTP status code applicable to this problem.\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"maxLength\": 500,\n      \"description\": \"A human-readable explanation specific\
  \ to this occurrence of the problem.\"\n    },\n    \"instance\": {\n      \"type\": \"string\",\n      \"maxLength\": 500,\n      \"description\": \"A URI reference that identifies the specific occurrence of the problem.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/princess-beef-heavy-industries/refs/heads/main/json-schema/error.json
tags:
- Commerce
- Documentation
- Editors
- Governance
- Platform
- Products
- Rules
title: pb33f Giftshop Error
---
