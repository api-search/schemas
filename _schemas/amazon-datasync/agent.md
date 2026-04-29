---
description: A DataSync agent deployed on-premises or in a VPC for data transfer.
layout: schema
name: Agent
properties_list:
- description: The ARN of the DataSync agent. This ARN uniquely identifies the agent.
  name: AgentArn
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: CreationTime
  type: string
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/agent-schema.json
slug: agent
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/agent-schema.json\",\n  \"title\": \"Agent\",\n  \"description\": \"A DataSync agent deployed on-premises or in a VPC for data transfer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AgentArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the DataSync agent. This ARN uniquely identifies the agent.\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ONLINE\",\n        \"OFFLINE\"\n      ]\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/agent-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Agent
---
