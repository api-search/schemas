---
description: An available FIS fault injection action
layout: schema
name: Action
properties_list:
- description: Action ID
  name: id
  type: string
- description: Action ARN
  name: arn
  type: string
- description: Action description
  name: description
  type: string
- description: Action parameters
  name: parameters
  type: object
- description: Target definitions
  name: targets
  type: object
- description: Resource tags
  name: tags
  type: object
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-action-schema.json
slug: amazon-fis-action
source_filename: amazon-fis-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"An available FIS fault injection action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Action ID\",\n      \"example\": \"aws:ec2:stop-instances\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"Action ARN\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Action description\",\n      \"example\": \"Stop EC2 instances\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Action parameters\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"targets\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Target definitions\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource tags\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-action-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: Action
---
