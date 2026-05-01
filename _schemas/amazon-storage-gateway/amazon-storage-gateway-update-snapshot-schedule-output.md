---
description: A JSON object containing the Amazon Resource Name (ARN) of the updated storage volume.
layout: schema
name: UpdateSnapshotScheduleOutput
properties_list:
- description: ''
  name: VolumeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-snapshot-schedule-output-schema.json
slug: amazon-storage-gateway-update-snapshot-schedule-output
source_filename: amazon-storage-gateway-update-snapshot-schedule-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-snapshot-schedule-output-schema.json\",\n  \"title\": \"UpdateSnapshotScheduleOutput\",\n  \"description\": \"A JSON object containing the Amazon Resource Name (ARN) of the updated storage volume.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume. Use the <a>ListVolumes</a> operation to return a list of gateway volumes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-snapshot-schedule-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateSnapshotScheduleOutput
---
