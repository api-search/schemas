---
description: DeleteSnapshotScheduleInput schema from Amazon Storage Gateway API
layout: schema
name: DeleteSnapshotScheduleInput
properties_list:
- description: ''
  name: VolumeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-snapshot-schedule-input-schema.json
slug: amazon-storage-gateway-delete-snapshot-schedule-input
source_filename: amazon-storage-gateway-delete-snapshot-schedule-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-snapshot-schedule-input-schema.json\",\n  \"title\": \"DeleteSnapshotScheduleInput\",\n  \"description\": \"DeleteSnapshotScheduleInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The volume which snapshot schedule to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VolumeARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-snapshot-schedule-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteSnapshotScheduleInput
---
