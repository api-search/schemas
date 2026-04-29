---
description: '<p>The status of a specified delivery channel.</p> <p>Valid values: <code>Success</code> | <code>Failure</code> </p>'
layout: schema
name: DeliveryChannelStatus
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: configSnapshotDeliveryInfo
  type: object
- description: ''
  name: configHistoryDeliveryInfo
  type: object
- description: ''
  name: configStreamDeliveryInfo
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delivery-channel-status-schema.json
slug: config-delivery-channel-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delivery-channel-status-schema.json\",\n  \"title\": \"DeliveryChannelStatus\",\n  \"description\": \"<p>The status of a specified delivery channel.</p> <p>Valid values: <code>Success</code> | <code>Failure</code> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the delivery channel.\"\n        }\n      ]\n    },\n    \"configSnapshotDeliveryInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigExportDeliveryInfo\"\n        },\n        {\n          \"description\": \"A list containing the status of the delivery of the snapshot to the specified Amazon S3 bucket.\"\n        }\n      ]\n    },\n\
  \    \"configHistoryDeliveryInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigExportDeliveryInfo\"\n        },\n        {\n          \"description\": \"A list that contains the status of the delivery of the configuration history to the specified Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"configStreamDeliveryInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigStreamDeliveryInfo\"\n        },\n        {\n          \"description\": \"A list containing the status of the delivery of the configuration stream notification to the specified Amazon SNS topic.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delivery-channel-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeliveryChannelStatus
---
