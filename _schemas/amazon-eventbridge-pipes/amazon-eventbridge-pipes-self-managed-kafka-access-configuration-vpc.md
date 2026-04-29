---
description: This structure specifies the VPC subnets and security groups for the stream, and whether a public IP address is to be used.
layout: schema
name: SelfManagedKafkaAccessConfigurationVpc
properties_list:
- description: ''
  name: SecurityGroup
  type: object
- description: ''
  name: Subnets
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-self-managed-kafka-access-configuration-vpc-schema.json
slug: amazon-eventbridge-pipes-self-managed-kafka-access-configuration-vpc
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-self-managed-kafka-access-configuration-vpc-schema.json\",\n  \"title\": \"SelfManagedKafkaAccessConfigurationVpc\",\n  \"description\": \"This structure specifies the VPC subnets and security groups for the stream, and whether a public IP address is to be used.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"Specifies the security groups associated with the stream. These security groups must all be in the same VPC. You can specify as many as five security groups. If you do not specify a security group, the default security group for the VPC is used.\"\n        }\n      ]\n    },\n    \"Subnets\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"Specifies the subnets associated with the stream. These subnets must all be in the same VPC. You can specify as many as 16 subnets.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-self-managed-kafka-access-configuration-vpc-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: SelfManagedKafkaAccessConfigurationVpc
---
