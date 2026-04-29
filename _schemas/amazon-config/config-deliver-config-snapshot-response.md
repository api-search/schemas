---
description: The output for the <a>DeliverConfigSnapshot</a> action, in JSON format.
layout: schema
name: DeliverConfigSnapshotResponse
properties_list:
- description: ''
  name: configSnapshotId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-deliver-config-snapshot-response-schema.json
slug: config-deliver-config-snapshot-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-deliver-config-snapshot-response-schema.json\",\n  \"title\": \"DeliverConfigSnapshotResponse\",\n  \"description\": \"The output for the <a>DeliverConfigSnapshot</a> action, in JSON format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configSnapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the snapshot that is being created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-deliver-config-snapshot-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeliverConfigSnapshotResponse
---
