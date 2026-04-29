---
description: A content view defining a curated set of repositories and content available to hosts.
layout: schema
name: ContentView
properties_list:
- description: Unique identifier for the content view.
  name: id
  type: integer
- description: Name of the content view.
  name: name
  type: string
- description: Unique label for the content view (auto-generated from name).
  name: label
  type: string
- description: Description of the content view.
  name: description
  type: '[''string'', ''null'']'
- description: Organization this content view belongs to.
  name: organization_id
  type: integer
- description: ''
  name: organization
  type: object
- description: Whether this is a composite content view combining other content view versions.
  name: composite
  type: boolean
- description: Whether this is a rolling content view.
  name: rolling
  type: boolean
- description: Whether composite content views auto-publish when a component is updated.
  name: auto_publish
  type: boolean
- description: Whether RPM dependencies are resolved during publish.
  name: solve_dependencies
  type: boolean
- description: Whether this content view is only for upstream imports.
  name: import_only
  type: boolean
- description: If generated, indicates the purpose (e.g., import or export).
  name: generated_for
  type: '[''string'', ''null'']'
- description: Whether this is the default content view (every organization has one).
  name: default
  type: boolean
- description: Identifiers of repositories in this content view.
  name: repository_ids
  type: array
- description: Repositories included in this content view.
  name: repositories
  type: array
- description: Content view version IDs for composite content views.
  name: component_ids
  type: array
- description: Published versions of this content view.
  name: versions
  type: array
- description: Lifecycle environments this content view is in.
  name: environments
  type: array
- description: Activation keys using this content view.
  name: activation_keys
  type: array
- description: Next version number to be published.
  name: next_version
  type: string
- description: Timestamp of the last publish.
  name: last_published
  type: '[''string'', ''null'']'
- description: Latest published version number.
  name: latest_version
  type: '[''string'', ''null'']'
- description: Identifier of the latest published version.
  name: latest_version_id
  type: '[''integer'', ''null'']'
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-content-view-schema.json
slug: red-hat-satellite-content-view
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentView\",\n  \"type\": \"object\",\n  \"description\": \"A content view defining a curated set of repositories and content available to hosts.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the content view.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the content view.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Unique label for the content view (auto-generated from name).\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Description of the content view.\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization this content view belongs to.\"\n    },\n    \"organization\": {\n      \"type\": \"object\"\n    },\n    \"composite\": {\n  \
  \    \"type\": \"boolean\",\n      \"description\": \"Whether this is a composite content view combining other content view versions.\"\n    },\n    \"rolling\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a rolling content view.\"\n    },\n    \"auto_publish\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether composite content views auto-publish when a component is updated.\"\n    },\n    \"solve_dependencies\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether RPM dependencies are resolved during publish.\"\n    },\n    \"import_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this content view is only for upstream imports.\"\n    },\n    \"generated_for\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"If generated, indicates the purpose (e.g., import or export).\"\n    },\n    \"default\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default\
  \ content view (every organization has one).\"\n    },\n    \"repository_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Identifiers of repositories in this content view.\"\n    },\n    \"repositories\": {\n      \"type\": \"array\",\n      \"description\": \"Repositories included in this content view.\"\n    },\n    \"component_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Content view version IDs for composite content views.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"Published versions of this content view.\"\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"Lifecycle environments this content view is in.\"\n    },\n    \"activation_keys\": {\n      \"type\": \"array\",\n      \"description\": \"Activation keys using this content view.\"\n    },\n    \"next_version\": {\n      \"type\": \"string\",\n      \"description\": \"Next version number to be published.\"\n    },\n  \
  \  \"last_published\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Timestamp of the last publish.\"\n    },\n    \"latest_version\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Latest published version number.\"\n    },\n    \"latest_version_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Identifier of the latest published version.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-content-view-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: ContentView
---
