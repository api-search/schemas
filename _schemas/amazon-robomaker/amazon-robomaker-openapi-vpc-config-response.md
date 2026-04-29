---
description: VPC configuration associated with your simulation job.
layout: schema
name: VPCConfigResponse
properties_list:
- description: ''
  name: subnets
  type: object
- description: ''
  name: securityGroups
  type: object
- description: ''
  name: vpcId
  type: object
- description: ''
  name: assignPublicIp
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-vpc-config-response-schema.json
slug: amazon-robomaker-openapi-vpc-config-response
source_filename: amazon-robomaker-openapi-vpc-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-vpc-config-response-schema.json\",\n  \"title\": \"VPCConfigResponse\",\n  \"description\": \"VPC configuration associated with your simulation job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subnets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Subnets\"\n        },\n        {\n          \"description\": \"A list of subnet IDs associated with the simulation job.\"\n        }\n      ]\n    },\n    \"securityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroups\"\n        },\n        {\n          \"description\": \"A list of security group IDs associated with the simulation job.\"\n        }\n      ]\n    },\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\
  \n        },\n        {\n          \"description\": \"The VPC ID associated with your simulation job.\"\n        }\n      ]\n    },\n    \"assignPublicIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A boolean indicating if a public IP was assigned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-vpc-config-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: VPCConfigResponse
---
