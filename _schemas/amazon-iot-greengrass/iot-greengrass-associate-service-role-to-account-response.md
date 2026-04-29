---
description: AssociateServiceRoleToAccountResponse schema
layout: schema
name: AssociateServiceRoleToAccountResponse
properties_list:
- description: ''
  name: associatedAt
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-associate-service-role-to-account-response-schema.json
slug: iot-greengrass-associate-service-role-to-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-service-role-to-account-response-schema.json\",\n  \"title\": \"AssociateServiceRoleToAccountResponse\",\n  \"description\": \"AssociateServiceRoleToAccountResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"AssociatedAt\"\n          },\n          \"description\": \"The time when the service role was associated with IoT Greengrass for your Amazon Web Services account in this Amazon Web Services Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-service-role-to-account-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: AssociateServiceRoleToAccountResponse
---
