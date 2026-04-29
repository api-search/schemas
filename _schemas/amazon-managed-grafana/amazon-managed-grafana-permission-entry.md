---
description: A structure containing the identity of one user or group and the <code>Admin</code>, <code>Editor</code>, or <code>Viewer</code> role that they have.
layout: schema
name: PermissionEntry
properties_list:
- description: ''
  name: role
  type: object
- description: ''
  name: user
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-permission-entry-schema.json
slug: amazon-managed-grafana-permission-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-permission-entry-schema.json\",\n  \"title\": \"PermissionEntry\",\n  \"description\": \"A structure containing the identity of one user or group and the <code>Admin</code>, <code>Editor</code>, or <code>Viewer</code> role that they have.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"Specifies whether the user or group has the <code>Admin</code>, <code>Editor</code>, or <code>Viewer</code> role.\"\n        }\n      ]\n    },\n    \"user\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/User\"\n        },\n        {\n          \"description\": \"A structure with the ID of the user or group with\
  \ this role.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"role\",\n    \"user\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-permission-entry-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: PermissionEntry
---
