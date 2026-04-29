---
description: Target definition in an experiment template
layout: schema
name: ExperimentTemplateTarget
properties_list:
- description: AWS resource type
  name: resourceType
  type: string
- description: Specific resource ARNs
  name: resourceArns
  type: array
- description: Tags to filter resources
  name: resourceTags
  type: object
- description: Resource filters
  name: filters
  type: array
- description: Selection mode
  name: selectionMode
  type: string
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-experiment-template-target-schema.json
slug: amazon-fis-experiment-template-target
source_filename: amazon-fis-experiment-template-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-target-schema.json\",\n  \"title\": \"ExperimentTemplateTarget\",\n  \"description\": \"Target definition in an experiment template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"AWS resource type\",\n      \"example\": \"aws:ec2:instance\"\n    },\n    \"resourceArns\": {\n      \"type\": \"array\",\n      \"description\": \"Specific resource ARNs\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"resourceTags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags to filter resources\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\":\
  \ \"Resource filters\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"selectionMode\": {\n      \"type\": \"string\",\n      \"description\": \"Selection mode\",\n      \"example\": \"ALL\",\n      \"enum\": [\n        \"ALL\",\n        \"COUNT(n)\",\n        \"PERCENT(n)\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-experiment-template-target-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: ExperimentTemplateTarget
---
