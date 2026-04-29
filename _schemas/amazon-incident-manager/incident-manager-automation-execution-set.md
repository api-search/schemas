---
description: AutomationExecutionSet schema
layout: schema
name: AutomationExecutionSet
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-automation-execution-set-schema.json
slug: incident-manager-automation-execution-set
source_filename: incident-manager-automation-execution-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-automation-execution-set-schema.json\",\n  \"title\": \"AutomationExecutionSet\",\n  \"description\": \"AutomationExecutionSet schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ssmExecutionArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of the automation process.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The Systems Manager automation document process to start as the runbook at the beginning of the incident.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-automation-execution-set-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: AutomationExecutionSet
---
