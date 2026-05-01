---
description: The input for the <a>DeliverConfigSnapshot</a> action.
layout: schema
name: DeliverConfigSnapshotRequest
properties_list:
- description: ''
  name: deliveryChannelName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-deliver-config-snapshot-request-schema.json
slug: config-deliver-config-snapshot-request
source_filename: config-deliver-config-snapshot-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-deliver-config-snapshot-request-schema.json\",\n  \"title\": \"DeliverConfigSnapshotRequest\",\n  \"description\": \"The input for the <a>DeliverConfigSnapshot</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deliveryChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelName\"\n        },\n        {\n          \"description\": \"The name of the delivery channel through which the snapshot is delivered.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deliveryChannelName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-deliver-config-snapshot-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DeliverConfigSnapshotRequest
---
