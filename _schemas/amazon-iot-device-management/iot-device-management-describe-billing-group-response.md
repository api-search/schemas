---
description: DescribeBillingGroupResponse schema
layout: schema
name: DescribeBillingGroupResponse
properties_list:
- description: ''
  name: billingGroupName
  type: object
- description: ''
  name: billingGroupId
  type: object
- description: ''
  name: billingGroupArn
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: billingGroupProperties
  type: object
- description: ''
  name: billingGroupMetadata
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-billing-group-response-schema.json
slug: iot-device-management-describe-billing-group-response
source_filename: iot-device-management-describe-billing-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-billing-group-response-schema.json\",\n  \"title\": \"DescribeBillingGroupResponse\",\n  \"description\": \"DescribeBillingGroupResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupName\"\n        },\n        {\n          \"description\": \"The name of the billing group.\"\n        }\n      ]\n    },\n    \"billingGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupId\"\n        },\n        {\n          \"description\": \"The ID of the billing group.\"\n        }\n      ]\n    },\n    \"billingGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupArn\"\
  \n        },\n        {\n          \"description\": \"The ARN of the billing group.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the billing group.\"\n        }\n      ]\n    },\n    \"billingGroupProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupProperties\"\n        },\n        {\n          \"description\": \"The properties of the billing group.\"\n        }\n      ]\n    },\n    \"billingGroupMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupMetadata\"\n        },\n        {\n          \"description\": \"Additional information about the billing group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-billing-group-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeBillingGroupResponse
---
