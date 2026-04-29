---
description: Specifies the minimum and maximum for the <code>MemoryMiB</code> object when you specify <a>InstanceRequirements</a> for an Auto Scaling group.
layout: schema
name: MemoryMiBRequest
properties_list:
- description: ''
  name: Min
  type: object
- description: ''
  name: Max
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-memory-mi-b-request-schema.json
slug: ec2-auto-scaling-memory-mi-b-request
source_filename: ec2-auto-scaling-memory-mi-b-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-memory-mi-b-request-schema.json\",\n  \"title\": \"MemoryMiBRequest\",\n  \"description\": \"Specifies the minimum and maximum for the <code>MemoryMiB</code> object when you specify <a>InstanceRequirements</a> for an Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Min\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullablePositiveInteger\"\n        },\n        {\n          \"description\": \"The memory minimum in MiB.\"\n        }\n      ]\n    },\n    \"Max\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullablePositiveInteger\"\n        },\n        {\n          \"description\": \"The memory maximum in MiB.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Min\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-memory-mi-b-request-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: MemoryMiBRequest
---
