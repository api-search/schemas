---
description: The input for the <a>DescribeDeliveryChannels</a> action.
layout: schema
name: DescribeDeliveryChannelsRequest
properties_list:
- description: ''
  name: DeliveryChannelNames
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-delivery-channels-request-schema.json
slug: config-describe-delivery-channels-request
source_filename: config-describe-delivery-channels-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channels-request-schema.json\",\n  \"title\": \"DescribeDeliveryChannelsRequest\",\n  \"description\": \"The input for the <a>DescribeDeliveryChannels</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryChannelNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryChannelNameList\"\n        },\n        {\n          \"description\": \"A list of delivery channel names.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channels-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeDeliveryChannelsRequest
---
