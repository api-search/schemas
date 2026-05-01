---
description: DescribeWorkspaceConfigurationResponse schema from Amazon Managed Grafana API
layout: schema
name: DescribeWorkspaceConfigurationResponse
properties_list:
- description: ''
  name: configuration
  type: object
- description: ''
  name: grafanaVersion
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-describe-workspace-configuration-response-schema.json
slug: amazon-managed-grafana-describe-workspace-configuration-response
source_filename: amazon-managed-grafana-describe-workspace-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-describe-workspace-configuration-response-schema.json\",\n  \"title\": \"DescribeWorkspaceConfigurationResponse\",\n  \"description\": \"DescribeWorkspaceConfigurationResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OverridableConfigurationJson\"\n        },\n        {\n          \"description\": \"The configuration string for the workspace that you requested. For more information about the format and configuration options available, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-configure-workspace.html\\\">Working in your Grafana workspace</a>.\"\n        }\n      ]\n    },\n    \"grafanaVersion\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrafanaVersion\"\n        },\n        {\n          \"description\": \"The supported Grafana version for the workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-describe-workspace-configuration-response-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: DescribeWorkspaceConfigurationResponse
---
