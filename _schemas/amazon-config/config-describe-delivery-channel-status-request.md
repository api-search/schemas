---
description: The input for the <a>DeliveryChannelStatus</a> action.
layout: schema
name: DescribeDeliveryChannelStatusRequest
properties_list:
- description: ''
  name: DeliveryChannelNames
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-delivery-channel-status-request-schema.json
slug: config-describe-delivery-channel-status-request
source_filename: config-describe-delivery-channel-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channel-status-request-schema.json\",\n  \"title\": \"DescribeDeliveryChannelStatusRequest\",\n  \"description\": \"The input for the <a>DeliveryChannelStatus</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryChannelNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryChannelNameList\"\n        },\n        {\n          \"description\": \"A list of delivery channel names.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channel-status-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeDeliveryChannelStatusRequest
---
