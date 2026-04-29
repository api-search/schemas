---
description: This structure defines which groups defined in the SAML assertion attribute are to be mapped to the Grafana <code>Admin</code> and <code>Editor</code> roles in the workspace. SAML authenticated users not part of <code>Admin</code> or <code>Editor</code> role groups have <code>Viewer</code> permission over the workspace.
layout: schema
name: RoleValues
properties_list:
- description: ''
  name: admin
  type: object
- description: ''
  name: editor
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-role-values-schema.json
slug: amazon-managed-grafana-role-values
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-role-values-schema.json\",\n  \"title\": \"RoleValues\",\n  \"description\": \"This structure defines which groups defined in the SAML assertion attribute are to be mapped to the Grafana <code>Admin</code> and <code>Editor</code> roles in the workspace. SAML authenticated users not part of <code>Admin</code> or <code>Editor</code> role groups have <code>Viewer</code> permission over the workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"admin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleValueList\"\n        },\n        {\n          \"description\": \"A list of groups from the SAML assertion attribute to grant the Grafana <code>Admin</code> role to.\"\n        }\n      ]\n    },\n    \"editor\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/RoleValueList\"\n        },\n        {\n          \"description\": \"A list of groups from the SAML assertion attribute to grant the Grafana <code>Editor</code> role to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-role-values-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: RoleValues
---
