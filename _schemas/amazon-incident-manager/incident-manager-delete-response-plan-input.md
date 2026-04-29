---
description: DeleteResponsePlanInput schema
layout: schema
name: DeleteResponsePlanInput
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-delete-response-plan-input-schema.json
slug: incident-manager-delete-response-plan-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-response-plan-input-schema.json\",\n  \"title\": \"DeleteResponsePlanInput\",\n  \"description\": \"DeleteResponsePlanInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the response plan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-response-plan-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: DeleteResponsePlanInput
---
