---
description: The Systems Manager automation document process to start as the runbook at the beginning of the incident.
layout: schema
name: AutomationExecution
properties_list:
- description: ''
  name: ssmExecutionArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-automation-execution-schema.json
slug: incident-manager-automation-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-automation-execution-schema.json\",\n  \"title\": \"AutomationExecution\",\n  \"description\": \"The Systems Manager automation document process to start as the runbook at the beginning of the incident.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ssmExecutionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the automation process.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-automation-execution-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: AutomationExecution
---
