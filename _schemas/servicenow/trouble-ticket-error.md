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
schema_file: json-schema/trouble-ticket-error-schema.json
slug: trouble-ticket-error
source_filename: trouble-ticket-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Error message\"\n        },\n        \"detail\": {\n          \"type\": \"string\",\n          \"description\": \"Detailed error information\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-error-schema.json
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
