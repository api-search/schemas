---
description: DeleteIncidentRecordInput schema
layout: schema
name: DeleteIncidentRecordInput
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-delete-incident-record-input-schema.json
slug: incident-manager-delete-incident-record-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-incident-record-input-schema.json\",\n  \"title\": \"DeleteIncidentRecordInput\",\n  \"description\": \"DeleteIncidentRecordInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident record you are deleting.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-incident-record-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: DeleteIncidentRecordInput
---
