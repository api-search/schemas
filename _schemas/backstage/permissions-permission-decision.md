---
description: PermissionDecision schema from Backstage permissions API
layout: schema
name: PermissionDecision
properties_list:
- description: The authorization decision result.
  name: result
  type: string
- description: The plugin responsible for condition evaluation.
  name: pluginId
  type: string
- description: The resource type for conditional decisions.
  name: resourceType
  type: string
- description: The conditions that must be evaluated against the resource to produce a final decision. Only present when result is CONDITIONAL.
  name: conditions
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/permissions-permission-decision-schema.json
slug: permissions-permission-decision
source_filename: permissions-permission-decision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/permissions-permission-decision-schema.json\",\n  \"title\": \"PermissionDecision\",\n  \"description\": \"PermissionDecision schema from Backstage permissions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ALLOW\",\n        \"DENY\",\n        \"CONDITIONAL\"\n      ],\n      \"description\": \"The authorization decision result.\"\n    },\n    \"pluginId\": {\n      \"type\": \"string\",\n      \"description\": \"The plugin responsible for condition evaluation.\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type for conditional decisions.\"\n    },\n    \"conditions\": {\n      \"type\": \"object\",\n      \"description\": \"The conditions that must be evaluated against\
  \ the resource to produce a final decision. Only present when result is CONDITIONAL.\"\n    }\n  },\n  \"required\": [\n    \"result\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/permissions-permission-decision-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: PermissionDecision
---
