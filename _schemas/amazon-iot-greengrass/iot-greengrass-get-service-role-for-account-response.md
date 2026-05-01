---
description: GetServiceRoleForAccountResponse schema
layout: schema
name: GetServiceRoleForAccountResponse
properties_list:
- description: ''
  name: associatedAt
  type: object
- description: ''
  name: roleArn
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-get-service-role-for-account-response-schema.json
slug: iot-greengrass-get-service-role-for-account-response
source_filename: iot-greengrass-get-service-role-for-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-service-role-for-account-response-schema.json\",\n  \"title\": \"GetServiceRoleForAccountResponse\",\n  \"description\": \"GetServiceRoleForAccountResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"AssociatedAt\"\n          },\n          \"description\": \"The time when the service role was associated with IoT Greengrass for your Amazon Web Services account in this Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"RoleArn\"\n          },\n          \"description\": \"The ARN of the service role that is associated with IoT Greengrass for your Amazon Web Services account in this Amazon Web Services Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-service-role-for-account-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: GetServiceRoleForAccountResponse
---
