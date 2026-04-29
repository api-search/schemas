---
description: An autolink reference.
layout: schema
name: autolink
properties_list:
- description: ''
  name: id
  type: integer
- description: The prefix of a key that is linkified.
  name: key_prefix
  type: string
- description: template for the target URL that is generated if a key was found.
  name: url_template
  type: string
- description: Whether this autolink reference matches alphanumeric characters. If false, this autolink reference only matches numeric characters.
  name: is_alphanumeric
  type: boolean
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-autolinks-api-autolink-schema.json
slug: github-repo-autolinks-api-autolink
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-autolinks-api-autolink-schema.json\",\n  \"title\": \"autolink\",\n  \"description\": \"An autolink reference.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 3\n    },\n    \"key_prefix\": {\n      \"description\": \"The prefix of a key that is linkified.\",\n      \"example\": \"TICKET-\",\n      \"type\": \"string\"\n    },\n    \"url_template\": {\n      \"description\": \"template for the target URL that is generated if a key was found.\",\n      \"example\": \"https://example.com/TICKET?query=<num>\",\n      \"type\": \"string\"\n    },\n    \"is_alphanumeric\": {\n      \"description\": \"Whether this autolink reference matches alphanumeric characters. If false, this autolink reference only matches numeric characters.\",\n    \
  \  \"example\": true,\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"key_prefix\",\n    \"url_template\",\n    \"is_alphanumeric\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-autolinks-api-autolink-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: autolink
---
