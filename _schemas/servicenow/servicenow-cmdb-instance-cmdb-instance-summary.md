---
description: A summary of a CMDB configuration item containing its identifier and display name.
layout: schema
name: CmdbInstanceSummary
properties_list:
- description: Unique identifier for the configuration item.
  name: sys_id
  type: string
- description: The display name of the configuration item.
  name: name
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-cmdb-instance-cmdb-instance-summary-schema.json
slug: servicenow-cmdb-instance-cmdb-instance-summary
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A summary of a CMDB configuration item containing its identifier and display name.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the configuration item.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the configuration item.\",\n      \"example\": \"Example Title\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CmdbInstanceSummary\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-cmdb-instance-cmdb-instance-summary-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: CmdbInstanceSummary
---
