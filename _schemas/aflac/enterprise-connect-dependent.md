---
description: A dependent to be covered under a family enrollment.
layout: schema
name: Dependent
properties_list:
- description: Dependent's first name.
  name: first_name
  type: string
- description: Dependent's last name.
  name: last_name
  type: string
- description: Dependent's date of birth.
  name: date_of_birth
  type: string
- description: Relationship to the employee.
  name: relationship
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-dependent-schema.json
slug: enterprise-connect-dependent
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-dependent-schema.json\",\n  \"title\": \"Dependent\",\n  \"description\": \"A dependent to be covered under a family enrollment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Dependent's first name.\",\n      \"example\": \"Jane\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Dependent's last name.\",\n      \"example\": \"Smith\"\n    },\n    \"date_of_birth\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Dependent's date of birth.\",\n      \"example\": \"1990-06-15\"\n    },\n    \"relationship\": {\n      \"type\": \"string\",\n      \"description\": \"Relationship to the employee.\",\n      \"enum\": [\n        \"spouse\",\n     \
  \   \"child\"\n      ],\n      \"example\": \"spouse\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-dependent-schema.json
tags: []
title: Dependent
---
