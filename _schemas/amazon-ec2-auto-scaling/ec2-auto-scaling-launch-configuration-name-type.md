---
description: LaunchConfigurationNameType schema from Auto Scaling
layout: schema
name: LaunchConfigurationNameType
properties_list:
- description: ''
  name: LaunchConfigurationName
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-launch-configuration-name-type-schema.json
slug: ec2-auto-scaling-launch-configuration-name-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-configuration-name-type-schema.json\",\n  \"title\": \"LaunchConfigurationNameType\",\n  \"description\": \"LaunchConfigurationNameType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the launch configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LaunchConfigurationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-configuration-name-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LaunchConfigurationNameType
---
