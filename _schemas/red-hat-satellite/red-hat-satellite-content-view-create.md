---
description: Parameters for creating a new content view.
layout: schema
name: ContentViewCreate
properties_list:
- description: Organization identifier.
  name: organization_id
  type: integer
- description: Name of the content view.
  name: name
  type: string
- description: Content view label (auto-generated from name if omitted).
  name: label
  type: string
- description: Description of the content view.
  name: description
  type: string
- description: Whether this is a composite content view.
  name: composite
  type: boolean
- description: Whether this is a rolling content view.
  name: rolling
  type: boolean
- description: Auto-publish composite view when a component updates.
  name: auto_publish
  type: boolean
- description: Resolve RPM dependencies during publish.
  name: solve_dependencies
  type: boolean
- description: Mark as import-only content view.
  name: import_only
  type: boolean
- description: Repository IDs to include.
  name: repository_ids
  type: array
- description: Content view version IDs for composite views.
  name: component_ids
  type: array
- description: Lifecycle environment IDs for rolling content views.
  name: environment_ids
  type: array
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-content-view-create-schema.json
slug: red-hat-satellite-content-view-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentViewCreate\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for creating a new content view.\",\n  \"properties\": {\n    \"organization_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the content view.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Content view label (auto-generated from name if omitted).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the content view.\"\n    },\n    \"composite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a composite content view.\"\n    },\n    \"rolling\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a rolling content view.\"\n    },\n    \"auto_publish\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Auto-publish composite view when a component updates.\"\n    },\n    \"solve_dependencies\": {\n      \"type\": \"boolean\",\n      \"description\": \"Resolve RPM dependencies during publish.\"\n    },\n    \"import_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Mark as import-only content view.\"\n    },\n    \"repository_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Repository IDs to include.\"\n    },\n    \"component_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Content view version IDs for composite views.\"\n    },\n    \"environment_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Lifecycle environment IDs for rolling content views.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-content-view-create-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: ContentViewCreate
---
