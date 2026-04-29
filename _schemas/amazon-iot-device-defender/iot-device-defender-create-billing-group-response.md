---
description: CreateBillingGroupResponse schema
layout: schema
name: CreateBillingGroupResponse
properties_list:
- description: ''
  name: billingGroupName
  type: object
- description: ''
  name: billingGroupArn
  type: object
- description: ''
  name: billingGroupId
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-billing-group-response-schema.json
slug: iot-device-defender-create-billing-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-billing-group-response-schema.json\",\n  \"title\": \"CreateBillingGroupResponse\",\n  \"description\": \"CreateBillingGroupResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupName\"\n        },\n        {\n          \"description\": \"The name you gave to the billing group.\"\n        }\n      ]\n    },\n    \"billingGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupArn\"\n        },\n        {\n          \"description\": \"The ARN of the billing group.\"\n        }\n      ]\n    },\n    \"billingGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupId\"\
  \n        },\n        {\n          \"description\": \"The ID of the billing group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-billing-group-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateBillingGroupResponse
---
