---
description: Amazon Virtual Private Cloud configuration details associated with your Lambda function.
layout: schema
name: VpcConfig
properties_list:
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SecurityGroups
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-vpc-config-schema.json
slug: guardduty-vpc-config
source_filename: guardduty-vpc-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-vpc-config-schema.json\",\n  \"title\": \"VpcConfig\",\n  \"description\": \"Amazon Virtual Private Cloud configuration details associated with your Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetIds\"\n          },\n          \"description\": \"The identifiers of the subnets that are associated with your Lambda function.\"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcId\"\n          },\n          \"description\": \"The identifier of the\
  \ Amazon Virtual Private Cloud.\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroups\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroups\"\n          },\n          \"description\": \"The identifier of the security group attached to the Lambda function.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-vpc-config-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: VpcConfig
---
