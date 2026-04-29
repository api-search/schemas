---
description: A structure containing information about the user authentication methods used by the workspace.
layout: schema
name: AuthenticationDescription
properties_list:
- description: ''
  name: awsSso
  type: object
- description: ''
  name: providers
  type: object
- description: ''
  name: saml
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-authentication-description-schema.json
slug: amazon-managed-grafana-authentication-description
source_filename: amazon-managed-grafana-authentication-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-authentication-description-schema.json\",\n  \"title\": \"AuthenticationDescription\",\n  \"description\": \"A structure containing information about the user authentication methods used by the workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsSso\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsSsoAuthentication\"\n        },\n        {\n          \"description\": \"A structure containing information about how this workspace works with IAM Identity Center. \"\n        }\n      ]\n    },\n    \"providers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationProviders\"\n        },\n        {\n          \"description\": \"Specifies whether this workspace uses IAM Identity Center, SAML,\
  \ or both methods to authenticate users to use the Grafana console in the Amazon Managed Grafana workspace.\"\n        }\n      ]\n    },\n    \"saml\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlAuthentication\"\n        },\n        {\n          \"description\": \"A structure containing information about how this workspace works with SAML, including what attributes within the assertion are to be mapped to user information in the workspace. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"providers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-authentication-description-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: AuthenticationDescription
---
