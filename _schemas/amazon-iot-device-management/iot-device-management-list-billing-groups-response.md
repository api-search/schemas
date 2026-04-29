---
description: ListBillingGroupsResponse schema
layout: schema
name: ListBillingGroupsResponse
properties_list:
- description: ''
  name: billingGroups
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-billing-groups-response-schema.json
slug: iot-device-management-list-billing-groups-response
source_filename: iot-device-management-list-billing-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-billing-groups-response-schema.json\",\n  \"title\": \"ListBillingGroupsResponse\",\n  \"description\": \"ListBillingGroupsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupNameAndArnList\"\n        },\n        {\n          \"description\": \"The list of billing groups.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-billing-groups-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListBillingGroupsResponse
---
