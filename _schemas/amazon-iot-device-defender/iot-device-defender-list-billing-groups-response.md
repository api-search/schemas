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
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-billing-groups-response-schema.json
slug: iot-device-defender-list-billing-groups-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-billing-groups-response-schema.json\",\n  \"title\": \"ListBillingGroupsResponse\",\n  \"description\": \"ListBillingGroupsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupNameAndArnList\"\n        },\n        {\n          \"description\": \"The list of billing groups.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-billing-groups-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListBillingGroupsResponse
---
