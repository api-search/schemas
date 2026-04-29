---
description: Specifies the minimum and maximum for the <code>NetworkInterfaceCount</code> object when you specify <a>InstanceRequirements</a> for an Auto Scaling group.
layout: schema
name: NetworkInterfaceCountRequest
properties_list:
- description: ''
  name: Min
  type: object
- description: ''
  name: Max
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-network-interface-count-request-schema.json
slug: ec2-auto-scaling-network-interface-count-request
source_filename: ec2-auto-scaling-network-interface-count-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-network-interface-count-request-schema.json\",\n  \"title\": \"NetworkInterfaceCountRequest\",\n  \"description\": \"Specifies the minimum and maximum for the <code>NetworkInterfaceCount</code> object when you specify <a>InstanceRequirements</a> for an Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Min\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullablePositiveInteger\"\n        },\n        {\n          \"description\": \"The minimum number of network interfaces.\"\n        }\n      ]\n    },\n    \"Max\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullablePositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of network interfaces.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-network-interface-count-request-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: NetworkInterfaceCountRequest
---
