---
description: Parameters for updating a content view.
layout: schema
name: ContentViewUpdate
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: auto_publish
  type: boolean
- description: ''
  name: solve_dependencies
  type: boolean
- description: ''
  name: repository_ids
  type: array
- description: ''
  name: component_ids
  type: array
- description: ''
  name: environment_ids
  type: array
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-content-view-update-schema.json
slug: red-hat-satellite-content-view-update
source_filename: red-hat-satellite-content-view-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentViewUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for updating a content view.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"auto_publish\": {\n      \"type\": \"boolean\"\n    },\n    \"solve_dependencies\": {\n      \"type\": \"boolean\"\n    },\n    \"repository_ids\": {\n      \"type\": \"array\"\n    },\n    \"component_ids\": {\n      \"type\": \"array\"\n    },\n    \"environment_ids\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-content-view-update-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: ContentViewUpdate
---
