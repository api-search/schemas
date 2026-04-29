---
description: AssociateServiceRoleToAccountRequest schema
layout: schema
name: AssociateServiceRoleToAccountRequest
properties_list:
- description: ''
  name: roleArn
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-associate-service-role-to-account-request-schema.json
slug: iot-greengrass-associate-service-role-to-account-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-service-role-to-account-request-schema.json\",\n  \"title\": \"AssociateServiceRoleToAccountRequest\",\n  \"description\": \"AssociateServiceRoleToAccountRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"RoleArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the service role to associate with IoT Greengrass for your Amazon Web Services account in this Amazon Web Services Region.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-service-role-to-account-request-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: AssociateServiceRoleToAccountRequest
---
