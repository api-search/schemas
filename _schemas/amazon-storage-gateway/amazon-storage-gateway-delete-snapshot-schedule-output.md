---
description: DeleteSnapshotScheduleOutput schema from Amazon Storage Gateway API
layout: schema
name: DeleteSnapshotScheduleOutput
properties_list:
- description: ''
  name: VolumeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-snapshot-schedule-output-schema.json
slug: amazon-storage-gateway-delete-snapshot-schedule-output
source_filename: amazon-storage-gateway-delete-snapshot-schedule-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-snapshot-schedule-output-schema.json\",\n  \"title\": \"DeleteSnapshotScheduleOutput\",\n  \"description\": \"DeleteSnapshotScheduleOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The volume which snapshot schedule was deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-snapshot-schedule-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteSnapshotScheduleOutput
---
