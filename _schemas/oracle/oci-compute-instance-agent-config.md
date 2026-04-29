---
description: Configuration options for the Oracle Cloud Agent software
layout: schema
name: InstanceAgentConfig
properties_list:
- description: Whether the Monitoring plugin is disabled
  name: isMonitoringDisabled
  type: boolean
- description: Whether the Management plugin is disabled
  name: isManagementDisabled
  type: boolean
- description: Whether all plugins are disabled
  name: areAllPluginsDisabled
  type: boolean
- description: The configuration of plugins associated with this instance
  name: pluginsConfig
  type: array
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-instance-agent-config-schema.json
slug: oci-compute-instance-agent-config
source_filename: oci-compute-instance-agent-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceAgentConfig\",\n  \"type\": \"object\",\n  \"description\": \"Configuration options for the Oracle Cloud Agent software\",\n  \"properties\": {\n    \"isMonitoringDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Monitoring plugin is disabled\"\n    },\n    \"isManagementDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Management plugin is disabled\"\n    },\n    \"areAllPluginsDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether all plugins are disabled\"\n    },\n    \"pluginsConfig\": {\n      \"type\": \"array\",\n      \"description\": \"The configuration of plugins associated with this instance\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-instance-agent-config-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: InstanceAgentConfig
---
