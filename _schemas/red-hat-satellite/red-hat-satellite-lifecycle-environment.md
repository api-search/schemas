---
description: A lifecycle environment defining a stage in the content promotion path.
layout: schema
name: LifecycleEnvironment
properties_list:
- description: Unique identifier for the lifecycle environment.
  name: id
  type: integer
- description: Name of the lifecycle environment.
  name: name
  type: string
- description: Unique label for the lifecycle environment.
  name: label
  type: string
- description: Description of the lifecycle environment.
  name: description
  type: '[''string'', ''null'']'
- description: Organization this environment belongs to.
  name: organization_id
  type: integer
- description: ''
  name: organization
  type: object
- description: Whether this is the Library environment.
  name: library
  type: boolean
- description: Prior environment in the promotion path.
  name: prior
  type: object
- description: Successor environment in the promotion path.
  name: successor
  type: '[''object'', ''null'']'
- description: Content counts for this environment.
  name: counts
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-lifecycle-environment-schema.json
slug: red-hat-satellite-lifecycle-environment
source_filename: red-hat-satellite-lifecycle-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleEnvironment\",\n  \"type\": \"object\",\n  \"description\": \"A lifecycle environment defining a stage in the content promotion path.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the lifecycle environment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the lifecycle environment.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Unique label for the lifecycle environment.\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Description of the lifecycle environment.\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization this environment belongs to.\"\n    },\n    \"organization\": {\n      \"type\": \"object\"\n    },\n    \"library\": {\n \
  \     \"type\": \"boolean\",\n      \"description\": \"Whether this is the Library environment.\"\n    },\n    \"prior\": {\n      \"type\": \"object\",\n      \"description\": \"Prior environment in the promotion path.\"\n    },\n    \"successor\": {\n      \"type\": \"['object', 'null']\",\n      \"description\": \"Successor environment in the promotion path.\"\n    },\n    \"counts\": {\n      \"type\": \"object\",\n      \"description\": \"Content counts for this environment.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-lifecycle-environment-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: LifecycleEnvironment
---
