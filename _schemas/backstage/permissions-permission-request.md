---
description: PermissionRequest schema from Backstage permissions API
layout: schema
name: PermissionRequest
properties_list:
- description: ''
  name: permission
  type: object
- description: Reference to the specific resource being accessed (e.g., component:default/my-service).
  name: resourceRef
  type: string
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/permissions-permission-request-schema.json
slug: permissions-permission-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/permissions-permission-request-schema.json\",\n  \"title\": \"PermissionRequest\",\n  \"description\": \"PermissionRequest schema from Backstage permissions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permission\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"type\",\n        \"name\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"basic\",\n            \"resource\"\n          ],\n          \"description\": \"The permission type.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The unique permission name.\"\n        },\n        \"resourceType\": {\n          \"type\": \"string\",\n          \"description\": \"The resource type for resource-based permissions.\"\
  \n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"action\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"create\",\n                \"read\",\n                \"update\",\n                \"delete\"\n              ],\n              \"description\": \"The action being performed.\"\n            }\n          }\n        }\n      }\n    },\n    \"resourceRef\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the specific resource being accessed (e.g., component:default/my-service).\"\n    }\n  },\n  \"required\": [\n    \"permission\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/permissions-permission-request-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: PermissionRequest
---
