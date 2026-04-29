---
description: Action definition in an experiment template
layout: schema
name: ExperimentTemplateAction
properties_list:
- description: FIS action ID
  name: actionId
  type: string
- description: Action description
  name: description
  type: string
- description: Action parameters
  name: parameters
  type: object
- description: Target mappings
  name: targets
  type: object
- description: Actions that must complete first
  name: startAfter
  type: array
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-experiment-template-action-schema.json
slug: amazon-fis-experiment-template-action
source_filename: amazon-fis-experiment-template-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-action-schema.json\",\n  \"title\": \"ExperimentTemplateAction\",\n  \"description\": \"Action definition in an experiment template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionId\": {\n      \"type\": \"string\",\n      \"description\": \"FIS action ID\",\n      \"example\": \"aws:ec2:stop-instances\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Action description\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Action parameters\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"targets\": {\n      \"type\": \"object\",\n      \"description\": \"Target mappings\",\n      \"additionalProperties\": {\n        \"type\"\
  : \"string\"\n      }\n    },\n    \"startAfter\": {\n      \"type\": \"array\",\n      \"description\": \"Actions that must complete first\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-action-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: ExperimentTemplateAction
---
