---
description: The metadata associated with the creation/updates to the user.
layout: schema
name: meta
properties_list:
- description: A type of a resource
  name: resourceType
  type: string
- description: A date and time when the user was created.
  name: created
  type: string
- description: A data and time when the user was last modified.
  name: lastModified
  type: string
- description: A URL location of an object
  name: location
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-scim-meta-schema.json
slug: github-scim-meta
source_filename: github-scim-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-meta-schema.json\",\n  \"title\": \"meta\",\n  \"description\": \"The metadata associated with the creation/updates to the user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"A type of a resource\",\n      \"enum\": [\n        \"User\",\n        \"Group\"\n      ],\n      \"example\": \"User\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"A date and time when the user was created.\",\n      \"example\": \"2022-03-27T19:59:26.000Z\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"description\": \"A data and time when the user was last modified.\",\n      \"example\": \"2022-03-27T19:59:26.000Z\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"A URL location of an object\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"resourceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-meta-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: meta
---
