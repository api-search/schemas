---
description: Contains the instructions for one Grafana role permission update in a <a href="https://docs.aws.amazon.com/grafana/latest/APIReference/API_UpdatePermissions.html">UpdatePermissions</a> operation.
layout: schema
name: UpdateInstruction
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: role
  type: object
- description: ''
  name: users
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-update-instruction-schema.json
slug: amazon-managed-grafana-update-instruction
source_filename: amazon-managed-grafana-update-instruction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-instruction-schema.json\",\n  \"title\": \"UpdateInstruction\",\n  \"description\": \"Contains the instructions for one Grafana role permission update in a <a href=\\\"https://docs.aws.amazon.com/grafana/latest/APIReference/API_UpdatePermissions.html\\\">UpdatePermissions</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateAction\"\n        },\n        {\n          \"description\": \"Specifies whether this update is to add or revoke role permissions.\"\n        }\n      ]\n    },\n    \"role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The role to add or revoke for\
  \ the user or the group specified in <code>users</code>.\"\n        }\n      ]\n    },\n    \"users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"A structure that specifies the user or group to add or revoke the role for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"role\",\n    \"users\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-instruction-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: UpdateInstruction
---
