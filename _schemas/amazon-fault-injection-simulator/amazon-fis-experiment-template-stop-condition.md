---
description: Stop condition for an experiment
layout: schema
name: ExperimentTemplateStopCondition
properties_list:
- description: Stop condition source
  name: source
  type: string
- description: CloudWatch alarm ARN or none
  name: value
  type: string
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-experiment-template-stop-condition-schema.json
slug: amazon-fis-experiment-template-stop-condition
source_filename: amazon-fis-experiment-template-stop-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-stop-condition-schema.json\",\n  \"title\": \"ExperimentTemplateStopCondition\",\n  \"description\": \"Stop condition for an experiment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Stop condition source\",\n      \"example\": \"aws:cloudwatch:alarm\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"CloudWatch alarm ARN or none\",\n      \"example\": \"arn:aws:cloudwatch:us-east-1:123456789012:alarm/my-alarm\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-stop-condition-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: ExperimentTemplateStopCondition
---
