---
description: An organization providing multi-tenancy isolation for content, hosts, and subscriptions.
layout: schema
name: Organization
properties_list:
- description: Unique identifier for the organization.
  name: id
  type: integer
- description: Organization name.
  name: name
  type: string
- description: Unique label for the organization.
  name: label
  type: string
- description: Organization title.
  name: title
  type: string
- description: Organization description.
  name: description
  type: '[''string'', ''null'']'
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-organization-schema.json
slug: red-hat-satellite-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Organization\",\n  \"type\": \"object\",\n  \"description\": \"An organization providing multi-tenancy isolation for content, hosts, and subscriptions.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the organization.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Unique label for the organization.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Organization title.\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Organization description.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-organization-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: Organization
---
