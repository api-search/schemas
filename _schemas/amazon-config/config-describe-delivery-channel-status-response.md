---
description: The output for the <a>DescribeDeliveryChannelStatus</a> action.
layout: schema
name: DescribeDeliveryChannelStatusResponse
properties_list:
- description: ''
  name: DeliveryChannelsStatus
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-delivery-channel-status-response-schema.json
slug: config-describe-delivery-channel-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channel-status-response-schema.json\",\n  \"title\": \"DescribeDeliveryChannelStatusResponse\",\n  \"description\": \"The output for the <a>DescribeDeliveryChannelStatus</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryChannelsStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryChannelStatusList\"\n        },\n        {\n          \"description\": \"A list that contains the status of a specified delivery channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channel-status-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeDeliveryChannelStatusResponse
---
