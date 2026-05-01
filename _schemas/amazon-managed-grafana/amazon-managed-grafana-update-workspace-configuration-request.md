---
description: UpdateWorkspaceConfigurationRequest schema from Amazon Managed Grafana API
layout: schema
name: UpdateWorkspaceConfigurationRequest
properties_list:
- description: ''
  name: configuration
  type: object
- description: ''
  name: grafanaVersion
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-update-workspace-configuration-request-schema.json
slug: amazon-managed-grafana-update-workspace-configuration-request
source_filename: amazon-managed-grafana-update-workspace-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-workspace-configuration-request-schema.json\",\n  \"title\": \"UpdateWorkspaceConfigurationRequest\",\n  \"description\": \"UpdateWorkspaceConfigurationRequest schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OverridableConfigurationJson\"\n        },\n        {\n          \"description\": \"The new configuration string for the workspace. For more information about the format and configuration options available, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-configure-workspace.html\\\">Working in your Grafana workspace</a>.\"\n        }\n      ]\n    },\n    \"grafanaVersion\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/GrafanaVersion\"\n        },\n        {\n          \"description\": \"<p>Specifies the version of Grafana to support in the new workspace.</p> <p>Can only be used to upgrade (for example, from 8.4 to 9.4), not downgrade (for example, from 9.4 to 8.4).</p> <p>To know what versions are available to upgrade to for a specific workspace, see the <code>ListVersions</code> operation.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-workspace-configuration-request-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: UpdateWorkspaceConfigurationRequest
---
