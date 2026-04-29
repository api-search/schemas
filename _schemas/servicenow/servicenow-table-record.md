---
description: A generic ServiceNow record. The actual fields depend on the table being queried. Common system fields are included in every record.
layout: schema
name: Record
properties_list:
- description: The unique 32-character system identifier for the record.
  name: sys_id
  type: string
- description: The date and time when the record was created.
  name: sys_created_on
  type: string
- description: The user who created the record.
  name: sys_created_by
  type: string
- description: The date and time when the record was last updated.
  name: sys_updated_on
  type: string
- description: The user who last updated the record.
  name: sys_updated_by
  type: string
- description: The number of times the record has been modified.
  name: sys_mod_count
  type: integer
- description: System tags associated with the record.
  name: sys_tags
  type: string
- description: The table class name for the record.
  name: sys_class_name
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-table-record-schema.json
slug: servicenow-table-record
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A generic ServiceNow record. The actual fields depend on the table being queried. Common system fields are included in every record.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique 32-character system identifier for the record.\",\n      \"example\": \"500123\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the record was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"sys_created_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the record.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the record was last updated.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n\
  \    \"sys_updated_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the record.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_mod_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times the record has been modified.\",\n      \"example\": 42\n    },\n    \"sys_tags\": {\n      \"type\": \"string\",\n      \"description\": \"System tags associated with the record.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_class_name\": {\n      \"type\": \"string\",\n      \"description\": \"The table class name for the record.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-table-record-schema.json
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
title: Record
---
