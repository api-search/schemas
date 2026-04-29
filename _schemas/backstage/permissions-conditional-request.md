---
description: ConditionalRequest schema from Backstage permissions API
layout: schema
name: ConditionalRequest
properties_list:
- description: Reference to the resource.
  name: resourceRef
  type: string
- description: The resource type identifier.
  name: resourceType
  type: string
- description: The conditions to evaluate against the resource.
  name: conditions
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/permissions-conditional-request-schema.json
slug: permissions-conditional-request
source_filename: permissions-conditional-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/permissions-conditional-request-schema.json\",\n  \"title\": \"ConditionalRequest\",\n  \"description\": \"ConditionalRequest schema from Backstage permissions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceRef\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the resource.\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"conditions\": {\n      \"type\": \"object\",\n      \"description\": \"The conditions to evaluate against the resource.\"\n    }\n  },\n  \"required\": [\n    \"resourceRef\",\n    \"resourceType\",\n    \"conditions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/permissions-conditional-request-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: ConditionalRequest
---
