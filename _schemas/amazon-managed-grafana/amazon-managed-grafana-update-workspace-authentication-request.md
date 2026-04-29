---
description: UpdateWorkspaceAuthenticationRequest schema from Amazon Managed Grafana API
layout: schema
name: UpdateWorkspaceAuthenticationRequest
properties_list:
- description: ''
  name: authenticationProviders
  type: object
- description: ''
  name: samlConfiguration
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-update-workspace-authentication-request-schema.json
slug: amazon-managed-grafana-update-workspace-authentication-request
source_filename: amazon-managed-grafana-update-workspace-authentication-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-workspace-authentication-request-schema.json\",\n  \"title\": \"UpdateWorkspaceAuthenticationRequest\",\n  \"description\": \"UpdateWorkspaceAuthenticationRequest schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationProviders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationProviders\"\n        },\n        {\n          \"description\": \"Specifies whether this workspace uses SAML 2.0, IAM Identity Center (successor to Single Sign-On), or both to authenticate users for using the Grafana console within a workspace. For more information, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/authentication-in-AMG.html\\\">User authentication in Amazon Managed\
  \ Grafana</a>.\"\n        }\n      ]\n    },\n    \"samlConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlConfiguration\"\n        },\n        {\n          \"description\": \"If the workspace uses SAML, use this structure to map SAML assertion attributes to workspace user information and define which groups in the assertion attribute are to have the <code>Admin</code> and <code>Editor</code> roles in the workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"authenticationProviders\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-workspace-authentication-request-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: UpdateWorkspaceAuthenticationRequest
---
