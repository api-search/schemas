---
description: A structure that specifies one user or group in the workspace.
layout: schema
name: User
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-user-schema.json
slug: amazon-managed-grafana-user
source_filename: amazon-managed-grafana-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A structure that specifies one user or group in the workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsoId\"\n        },\n        {\n          \"description\": \"<p>The ID of the user or group.</p> <p>Pattern: <code>^([0-9a-fA-F]{10}-|)[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$</code> </p>\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserType\"\n        },\n        {\n          \"description\": \"Specifies whether this is a single user or a group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"id\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-user-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: User
---
