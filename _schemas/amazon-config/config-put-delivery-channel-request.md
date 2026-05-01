---
description: The input for the <a>PutDeliveryChannel</a> action.
layout: schema
name: PutDeliveryChannelRequest
properties_list:
- description: ''
  name: DeliveryChannel
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-delivery-channel-request-schema.json
slug: config-put-delivery-channel-request
source_filename: config-put-delivery-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-delivery-channel-request-schema.json\",\n  \"title\": \"PutDeliveryChannelRequest\",\n  \"description\": \"The input for the <a>PutDeliveryChannel</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryChannel\"\n        },\n        {\n          \"description\": \"The configuration delivery channel object that delivers the configuration information to an Amazon S3 bucket and to an Amazon SNS topic.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeliveryChannel\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-delivery-channel-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutDeliveryChannelRequest
---
