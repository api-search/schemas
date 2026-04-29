---
description: A structure containing information about how this workspace works with SAML.
layout: schema
name: SamlAuthentication
properties_list:
- description: ''
  name: configuration
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-saml-authentication-schema.json
slug: amazon-managed-grafana-saml-authentication
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-saml-authentication-schema.json\",\n  \"title\": \"SamlAuthentication\",\n  \"description\": \"A structure containing information about how this workspace works with SAML. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlConfiguration\"\n        },\n        {\n          \"description\": \"A structure containing details about how this workspace works with SAML. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlConfigurationStatus\"\n        },\n        {\n          \"description\": \"Specifies whether the workspace's SAML configuration is complete.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-saml-authentication-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: SamlAuthentication
---
