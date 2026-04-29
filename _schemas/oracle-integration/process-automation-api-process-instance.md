---
description: ProcessInstance schema from Oracle Integration Process Automation API.
layout: schema
name: ProcessInstance
properties_list:
- description: Process instance identifier.
  name: processId
  type: string
- description: Process name.
  name: processName
  type: string
- description: Process definition identifier.
  name: processDefId
  type: string
- description: Process state.
  name: state
  type: string
- description: Process priority.
  name: priority
  type: integer
- description: Process title.
  name: title
  type: string
- description: User who created the instance.
  name: createdBy
  type: string
- description: Creation timestamp.
  name: createdDate
  type: string
provider_name: Oracle Integration
provider_slug: oracle-integration
schema_file: json-schema/process-automation-api-process-instance-schema.json
slug: process-automation-api-process-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/process-automation-api-process-instance-schema.json\",\n  \"title\": \"ProcessInstance\",\n  \"description\": \"ProcessInstance schema from Oracle Integration Process Automation API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"processId\": {\"type\": \"string\", \"description\": \"Process instance identifier.\"},\n    \"processName\": {\"type\": \"string\", \"description\": \"Process name.\"},\n    \"processDefId\": {\"type\": \"string\", \"description\": \"Process definition identifier.\"},\n    \"state\": {\"type\": \"string\", \"description\": \"Process state.\", \"enum\": [\"OPEN\", \"COMPLETED\", \"FAULTED\", \"ABORTED\"]},\n    \"priority\": {\"type\": \"integer\", \"description\": \"Process priority.\"},\n    \"title\": {\"type\": \"string\", \"description\": \"Process title.\"},\n\
  \    \"createdBy\": {\"type\": \"string\", \"description\": \"User who created the instance.\"},\n    \"createdDate\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Creation timestamp.\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/process-automation-api-process-instance-schema.json
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
title: ProcessInstance
---
