---
description: CreateSnapshotFromVolumeRecoveryPointOutput schema from Amazon Storage Gateway API
layout: schema
name: CreateSnapshotFromVolumeRecoveryPointOutput
properties_list:
- description: ''
  name: SnapshotId
  type: object
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: VolumeRecoveryPointTime
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-snapshot-from-volume-recovery-point-output-schema.json
slug: amazon-storage-gateway-create-snapshot-from-volume-recovery-point-output
source_filename: amazon-storage-gateway-create-snapshot-from-volume-recovery-point-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-snapshot-from-volume-recovery-point-output-schema.json\",\n  \"title\": \"CreateSnapshotFromVolumeRecoveryPointOutput\",\n  \"description\": \"CreateSnapshotFromVolumeRecoveryPointOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotId\"\n        },\n        {\n          \"description\": \"The ID of the snapshot.\"\n        }\n      ]\n    },\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the iSCSI volume target. Use the <a>DescribeStorediSCSIVolumes</a> operation to return\
  \ to retrieve the TargetARN for specified VolumeARN.\"\n        }\n      ]\n    },\n    \"VolumeRecoveryPointTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The time the volume was created from the recovery point.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-snapshot-from-volume-recovery-point-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateSnapshotFromVolumeRecoveryPointOutput
---
