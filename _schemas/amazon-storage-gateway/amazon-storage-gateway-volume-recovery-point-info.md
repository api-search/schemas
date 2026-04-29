---
description: Describes a storage volume recovery point object.
layout: schema
name: VolumeRecoveryPointInfo
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: VolumeSizeInBytes
  type: object
- description: ''
  name: VolumeUsageInBytes
  type: object
- description: ''
  name: VolumeRecoveryPointTime
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-volume-recovery-point-info-schema.json
slug: amazon-storage-gateway-volume-recovery-point-info
source_filename: amazon-storage-gateway-volume-recovery-point-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-volume-recovery-point-info-schema.json\",\n  \"title\": \"VolumeRecoveryPointInfo\",\n  \"description\": \"Describes a storage volume recovery point object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume target.\"\n        }\n      ]\n    },\n    \"VolumeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"The size of the volume in bytes.\"\n        }\n      ]\n    },\n    \"VolumeUsageInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\
  \n        },\n        {\n          \"description\": \"<p>The size of the data stored on the volume in bytes.</p> <note> <p>This value is not available for volumes created prior to May 13, 2015, until you store data on the volume.</p> </note>\"\n        }\n      ]\n    },\n    \"VolumeRecoveryPointTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The time the recovery point was taken.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-volume-recovery-point-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: VolumeRecoveryPointInfo
---
