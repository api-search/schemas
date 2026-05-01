---
description: SetInstanceProtectionQuery schema from Auto Scaling
layout: schema
name: SetInstanceProtectionQuery
properties_list:
- description: ''
  name: InstanceIds
  type: object
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: ProtectedFromScaleIn
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-set-instance-protection-query-schema.json
slug: ec2-auto-scaling-set-instance-protection-query
source_filename: ec2-auto-scaling-set-instance-protection-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-set-instance-protection-query-schema.json\",\n  \"title\": \"SetInstanceProtectionQuery\",\n  \"description\": \"SetInstanceProtectionQuery schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceIds\"\n        },\n        {\n          \"description\": \"One or more instance IDs. You can specify up to 50 instances.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"ProtectedFromScaleIn\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/ProtectedFromScaleIn\"\n        },\n        {\n          \"description\": \"Indicates whether the instance is protected from termination by Amazon EC2 Auto Scaling when scaling in.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceIds\",\n    \"AutoScalingGroupName\",\n    \"ProtectedFromScaleIn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-set-instance-protection-query-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: SetInstanceProtectionQuery
---
