---
description: If your simulation job accesses resources in a VPC, you provide this parameter identifying the list of security group IDs and subnet IDs. These must belong to the same VPC. You must provide at least one security group and two subnet IDs.
layout: schema
name: VPCConfig
properties_list:
- description: ''
  name: subnets
  type: object
- description: ''
  name: securityGroups
  type: object
- description: ''
  name: assignPublicIp
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-vpc-config-schema.json
slug: amazon-robomaker-openapi-vpc-config
source_filename: amazon-robomaker-openapi-vpc-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-vpc-config-schema.json\",\n  \"title\": \"VPCConfig\",\n  \"description\": \"If your simulation job accesses resources in a VPC, you provide this parameter identifying the list of security group IDs and subnet IDs. These must belong to the same VPC. You must provide at least one security group and two subnet IDs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subnets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Subnets\"\n        },\n        {\n          \"description\": \"A list of one or more subnet IDs in your VPC.\"\n        }\n      ]\n    },\n    \"securityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroups\"\n        },\n        {\n          \"description\": \"A list of one or\
  \ more security groups IDs in your VPC.\"\n        }\n      ]\n    },\n    \"assignPublicIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A boolean indicating whether to assign a public IP address.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"subnets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-vpc-config-schema.json
tags:
- AWS
- Robotics
- Simulation
title: VPCConfig
---
