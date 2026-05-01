---
description: The output for the <a>DescribeDeliveryChannels</a> action.
layout: schema
name: DescribeDeliveryChannelsResponse
properties_list:
- description: ''
  name: DeliveryChannels
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-delivery-channels-response-schema.json
slug: config-describe-delivery-channels-response
source_filename: config-describe-delivery-channels-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channels-response-schema.json\",\n  \"title\": \"DescribeDeliveryChannelsResponse\",\n  \"description\": \"The output for the <a>DescribeDeliveryChannels</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryChannels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryChannelList\"\n        },\n        {\n          \"description\": \"A list that contains the descriptions of the specified delivery channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-delivery-channels-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeDeliveryChannelsResponse
---
