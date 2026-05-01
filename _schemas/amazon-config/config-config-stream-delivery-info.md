---
description: A list that contains the status of the delivery of the configuration stream notification to the Amazon SNS topic.
layout: schema
name: ConfigStreamDeliveryInfo
properties_list:
- description: ''
  name: lastStatus
  type: object
- description: ''
  name: lastErrorCode
  type: object
- description: ''
  name: lastErrorMessage
  type: object
- description: ''
  name: lastStatusChangeTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-config-stream-delivery-info-schema.json
slug: config-config-stream-delivery-info
source_filename: config-config-stream-delivery-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-stream-delivery-info-schema.json\",\n  \"title\": \"ConfigStreamDeliveryInfo\",\n  \"description\": \"A list that contains the status of the delivery of the configuration stream notification to the Amazon SNS topic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryStatus\"\n        },\n        {\n          \"description\": \"<p>Status of the last attempted delivery.</p> <p> <b>Note</b> Providing an SNS topic on a <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_DeliveryChannel.html\\\">DeliveryChannel</a> for Config is optional. If the SNS delivery is turned off, the last status will be <b>Not_Applicable</b>.</p>\"\n        }\n      ]\n    },\n    \"lastErrorCode\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error code from the last attempted delivery.\"\n        }\n      ]\n    },\n    \"lastErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message from the last attempted delivery.\"\n        }\n      ]\n    },\n    \"lastStatusChangeTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time from the last status change.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-stream-delivery-info-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigStreamDeliveryInfo
---
