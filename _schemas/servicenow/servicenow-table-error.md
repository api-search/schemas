---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: error
  type: object
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-table-error-schema.json
slug: servicenow-table-error
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable error message.\"\n        },\n        \"detail\": {\n          \"type\": \"string\",\n          \"description\": \"Detailed information about the error.\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-table-error-schema.json
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
title: Error
---
