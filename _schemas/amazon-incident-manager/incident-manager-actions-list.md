---
description: ActionsList schema
layout: schema
name: ActionsList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-actions-list-schema.json
slug: incident-manager-actions-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-actions-list-schema.json\",\n  \"title\": \"ActionsList\",\n  \"description\": \"ActionsList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ssmAutomation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SsmAutomation\"\n          },\n          {\n            \"description\": \"The Systems Manager automation document to start as the runbook at the beginning of the incident.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The action that starts at the beginning of an incident. The response plan defines the action.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-actions-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ActionsList
---
