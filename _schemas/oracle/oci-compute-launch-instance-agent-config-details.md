---
description: Configuration options for the Oracle Cloud Agent on launch
layout: schema
name: LaunchInstanceAgentConfigDetails
properties_list:
- description: Whether to disable the Monitoring plugin
  name: isMonitoringDisabled
  type: boolean
- description: Whether to disable the Management plugin
  name: isManagementDisabled
  type: boolean
- description: Whether to disable all plugins
  name: areAllPluginsDisabled
  type: boolean
- description: Plugin configuration details
  name: pluginsConfig
  type: array
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-launch-instance-agent-config-details-schema.json
slug: oci-compute-launch-instance-agent-config-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LaunchInstanceAgentConfigDetails\",\n  \"type\": \"object\",\n  \"description\": \"Configuration options for the Oracle Cloud Agent on launch\",\n  \"properties\": {\n    \"isMonitoringDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable the Monitoring plugin\"\n    },\n    \"isManagementDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable the Management plugin\"\n    },\n    \"areAllPluginsDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable all plugins\"\n    },\n    \"pluginsConfig\": {\n      \"type\": \"array\",\n      \"description\": \"Plugin configuration details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-launch-instance-agent-config-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: LaunchInstanceAgentConfigDetails
---
