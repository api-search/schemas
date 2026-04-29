---
description: A structure that describes whether the workspace uses SAML, IAM Identity Center, or both methods for user authentication, and whether that authentication is fully configured.
layout: schema
name: AuthenticationSummary
properties_list:
- description: ''
  name: providers
  type: object
- description: ''
  name: samlConfigurationStatus
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-authentication-summary-schema.json
slug: amazon-managed-grafana-authentication-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-authentication-summary-schema.json\",\n  \"title\": \"AuthenticationSummary\",\n  \"description\": \"A structure that describes whether the workspace uses SAML, IAM Identity Center, or both methods for user authentication, and whether that authentication is fully configured.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"providers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationProviders\"\n        },\n        {\n          \"description\": \"Specifies whether the workspace uses SAML, IAM Identity Center, or both methods for user authentication.\"\n        }\n      ]\n    },\n    \"samlConfigurationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlConfigurationStatus\"\n        },\n\
  \        {\n          \"description\": \"Specifies whether the workplace's user authentication method is fully configured.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"providers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-authentication-summary-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: AuthenticationSummary
---
