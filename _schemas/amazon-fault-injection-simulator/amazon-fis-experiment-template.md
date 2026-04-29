---
description: An experiment template defining fault injection targets, actions, and stop conditions
layout: schema
name: ExperimentTemplate
properties_list:
- description: Template ID
  name: id
  type: string
- description: Template ARN
  name: arn
  type: string
- description: Template description
  name: description
  type: string
- description: Target definitions
  name: targets
  type: object
- description: Action definitions
  name: actions
  type: object
- description: Stop conditions
  name: stopConditions
  type: array
- description: Template creation time
  name: creationTime
  type: string
- description: Last update time
  name: lastUpdateTime
  type: string
- description: IAM role ARN for experiment execution
  name: roleArn
  type: string
- description: Resource tags
  name: tags
  type: object
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-experiment-template-schema.json
slug: amazon-fis-experiment-template
source_filename: amazon-fis-experiment-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-schema.json\",\n  \"title\": \"ExperimentTemplate\",\n  \"description\": \"An experiment template defining fault injection targets, actions, and stop conditions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID\",\n      \"example\": \"EXT123\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"Template ARN\",\n      \"example\": \"arn:aws:fis:us-east-1:123456789012:experiment-template/EXT123\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description\",\n      \"example\": \"Test EC2 instance failure\"\n    },\n    \"targets\": {\n      \"type\": \"object\",\n      \"description\": \"Target definitions\"\
  ,\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/ExperimentTemplateTarget\"\n      }\n    },\n    \"actions\": {\n      \"type\": \"object\",\n      \"description\": \"Action definitions\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/ExperimentTemplateAction\"\n      }\n    },\n    \"stopConditions\": {\n      \"type\": \"array\",\n      \"description\": \"Stop conditions\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExperimentTemplateStopCondition\"\n      }\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Template creation time\",\n      \"example\": \"2026-04-19T12:00:00Z\"\n    },\n    \"lastUpdateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update time\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role ARN for experiment execution\"\
  \n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource tags\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: ExperimentTemplate
---
