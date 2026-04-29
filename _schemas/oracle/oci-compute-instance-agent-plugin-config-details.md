---
description: Configuration details for an Oracle Cloud Agent plugin
layout: schema
name: InstanceAgentPluginConfigDetails
properties_list:
- description: The plugin name (e.g., Vulnerability Scanning, Bastion)
  name: name
  type: string
- description: Whether the plugin should be enabled or disabled
  name: desiredState
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-instance-agent-plugin-config-details-schema.json
slug: oci-compute-instance-agent-plugin-config-details
source_filename: oci-compute-instance-agent-plugin-config-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceAgentPluginConfigDetails\",\n  \"type\": \"object\",\n  \"description\": \"Configuration details for an Oracle Cloud Agent plugin\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The plugin name (e.g., Vulnerability Scanning, Bastion)\"\n    },\n    \"desiredState\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the plugin should be enabled or disabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-instance-agent-plugin-config-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: InstanceAgentPluginConfigDetails
---
