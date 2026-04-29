---
description: A workspace is the highest-level organizational unit in Asana. All projects and tasks have an associated workspace. An organization is a special kind of workspace that represents a company.
layout: schema
name: Asana Workspace
properties_list:
- description: Globally unique identifier of the resource.
  name: gid
  type: string
- description: The base type of this resource.
  name: resource_type
  type: string
- description: The name of the workspace.
  name: name
  type: string
- description: Whether the workspace is an organization.
  name: is_organization
  type: boolean
- description: The email domains associated with this workspace.
  name: email_domains
  type: array
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-workspace-json-schema.json
slug: asana-workspace-json
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developers.asana.com/schemas/workspace\",\n  \"title\": \"Asana Workspace\",\n  \"description\": \"A workspace is the highest-level organizational unit in Asana. All projects and tasks have an associated workspace. An organization is a special kind of workspace that represents a company.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gid\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique identifier of the resource.\",\n      \"readOnly\": true,\n      \"examples\": [\"12345\"]\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"const\": \"workspace\",\n      \"description\": \"The base type of this resource.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workspace.\",\n      \"examples\": [\"My Company Workspace\"]\n    },\n    \"is_organization\": {\n   \
  \   \"type\": \"boolean\",\n      \"description\": \"Whether the workspace is an organization.\",\n      \"readOnly\": true\n    },\n    \"email_domains\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"The email domains associated with this workspace.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"gid\", \"resource_type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/asana/refs/heads/main/json-schema/asana-workspace-json-schema.json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana Workspace
---
