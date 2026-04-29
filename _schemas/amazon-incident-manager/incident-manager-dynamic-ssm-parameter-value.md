---
description: The dynamic SSM parameter value.
layout: schema
name: DynamicSsmParameterValue
properties_list:
- description: ''
  name: variable
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-dynamic-ssm-parameter-value-schema.json
slug: incident-manager-dynamic-ssm-parameter-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-dynamic-ssm-parameter-value-schema.json\",\n  \"title\": \"DynamicSsmParameterValue\",\n  \"description\": \"The dynamic SSM parameter value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"variable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VariableType\"\n        },\n        {\n          \"description\": \"Variable dynamic parameters. A parameter value is determined when an incident is created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-dynamic-ssm-parameter-value-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: DynamicSsmParameterValue
---
