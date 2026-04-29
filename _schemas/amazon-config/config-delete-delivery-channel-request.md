---
description: The input for the <a>DeleteDeliveryChannel</a> action. The action accepts the following data, in JSON format.
layout: schema
name: DeleteDeliveryChannelRequest
properties_list:
- description: ''
  name: DeliveryChannelName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-delivery-channel-request-schema.json
slug: config-delete-delivery-channel-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-delivery-channel-request-schema.json\",\n  \"title\": \"DeleteDeliveryChannelRequest\",\n  \"description\": \"The input for the <a>DeleteDeliveryChannel</a> action. The action accepts the following data, in JSON format. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelName\"\n        },\n        {\n          \"description\": \"The name of the delivery channel to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeliveryChannelName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-delivery-channel-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteDeliveryChannelRequest
---
