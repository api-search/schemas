---
description: ''
layout: schema
name: ChannelInput
properties_list:
- description: Name of the contact method (can provide choice label or value, e.g., 'Virtual Agent' or 'virtual_agent')
  name: name
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-channel-input-schema.json
slug: trouble-ticket-channel-input
source_filename: trouble-ticket-channel-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the contact method (can provide choice label or value, e.g., 'Virtual Agent' or 'virtual_agent')\",\n      \"example\": \"Example Title\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChannelInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-channel-input-schema.json
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
title: ChannelInput
---
