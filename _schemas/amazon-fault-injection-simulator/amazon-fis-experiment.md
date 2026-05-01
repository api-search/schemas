---
description: A fault injection experiment instance
layout: schema
name: Experiment
properties_list:
- description: Experiment ID
  name: id
  type: string
- description: Experiment ARN
  name: arn
  type: string
- description: Source template ID
  name: experimentTemplateId
  type: string
- description: IAM role used
  name: roleArn
  type: string
- description: ''
  name: state
  type: object
- description: Resolved targets
  name: targets
  type: object
- description: Experiment actions
  name: actions
  type: object
- description: Stop conditions
  name: stopConditions
  type: array
- description: Experiment start time
  name: startTime
  type: string
- description: Experiment end time
  name: endTime
  type: string
- description: Resource tags
  name: tags
  type: object
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-experiment-schema.json
slug: amazon-fis-experiment
source_filename: amazon-fis-experiment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-schema.json\",\n  \"title\": \"Experiment\",\n  \"description\": \"A fault injection experiment instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Experiment ID\",\n      \"example\": \"EXP123\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"Experiment ARN\",\n      \"example\": \"arn:aws:fis:us-east-1:123456789012:experiment/EXP123\"\n    },\n    \"experimentTemplateId\": {\n      \"type\": \"string\",\n      \"description\": \"Source template ID\",\n      \"example\": \"EXT123\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role used\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/ExperimentState\"\
  \n    },\n    \"targets\": {\n      \"type\": \"object\",\n      \"description\": \"Resolved targets\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"actions\": {\n      \"type\": \"object\",\n      \"description\": \"Experiment actions\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"stopConditions\": {\n      \"type\": \"array\",\n      \"description\": \"Stop conditions\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Experiment start time\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Experiment end time\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource tags\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-schema.json
tags:
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: Experiment
---
