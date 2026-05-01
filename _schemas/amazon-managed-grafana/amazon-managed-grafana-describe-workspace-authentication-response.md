---
description: DescribeWorkspaceAuthenticationResponse schema from Amazon Managed Grafana API
layout: schema
name: DescribeWorkspaceAuthenticationResponse
properties_list:
- description: ''
  name: authentication
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-describe-workspace-authentication-response-schema.json
slug: amazon-managed-grafana-describe-workspace-authentication-response
source_filename: amazon-managed-grafana-describe-workspace-authentication-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-describe-workspace-authentication-response-schema.json\",\n  \"title\": \"DescribeWorkspaceAuthenticationResponse\",\n  \"description\": \"DescribeWorkspaceAuthenticationResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationDescription\"\n        },\n        {\n          \"description\": \"A structure containing information about the authentication methods used in the workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"authentication\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-describe-workspace-authentication-response-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: DescribeWorkspaceAuthenticationResponse
---
