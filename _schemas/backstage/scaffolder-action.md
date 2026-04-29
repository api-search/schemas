---
description: Action schema from Backstage scaffolder API
layout: schema
name: Action
properties_list:
- description: The unique identifier of the action.
  name: id
  type: string
- description: A human-readable description of the action.
  name: description
  type: string
- description: ''
  name: schema
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/scaffolder-action-schema.json
slug: scaffolder-action
source_filename: scaffolder-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/scaffolder-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"Action schema from Backstage scaffolder API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the action.\",\n      \"example\": \"fetch:plain\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the action.\"\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"input\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema for the action input.\"\n        },\n        \"output\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema for the action output.\"\n        }\n      }\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/scaffolder-action-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: Action
---
