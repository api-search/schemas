---
description: An available target resource type for FIS experiments
layout: schema
name: TargetResourceType
properties_list:
- description: Resource type identifier
  name: resourceType
  type: string
- description: Resource type description
  name: description
  type: string
- description: Resource type parameters
  name: parameters
  type: object
provider_name: Amazon Fault Injection Simulator
provider_slug: amazon-fault-injection-simulator
schema_file: json-schema/amazon-fis-target-resource-type-schema.json
slug: amazon-fis-target-resource-type
source_filename: amazon-fis-target-resource-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-target-resource-type-schema.json\",\n  \"title\": \"TargetResourceType\",\n  \"description\": \"An available target resource type for FIS experiments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier\",\n      \"example\": \"aws:ec2:instance\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type description\",\n      \"example\": \"EC2 Instance\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Resource type parameters\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fault-injection-simulator/refs/heads/main/json-schema/amazon-fis-target-resource-type-schema.json
tags:
- AWS
- Chaos Engineering
- DevOps
- Fault Injection
- Resilience Testing
title: TargetResourceType
---
