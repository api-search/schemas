---
description: DisassociateServiceRoleFromAccountResponse schema
layout: schema
name: DisassociateServiceRoleFromAccountResponse
properties_list:
- description: ''
  name: disassociatedAt
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-disassociate-service-role-from-account-response-schema.json
slug: iot-greengrass-disassociate-service-role-from-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-disassociate-service-role-from-account-response-schema.json\",\n  \"title\": \"DisassociateServiceRoleFromAccountResponse\",\n  \"description\": \"DisassociateServiceRoleFromAccountResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disassociatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"DisassociatedAt\"\n          },\n          \"description\": \"The time when the service role was disassociated from IoT Greengrass for your Amazon Web Services account in this Amazon Web Services Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-disassociate-service-role-from-account-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DisassociateServiceRoleFromAccountResponse
---
