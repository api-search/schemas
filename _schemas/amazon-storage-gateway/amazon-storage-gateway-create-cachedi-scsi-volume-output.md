---
description: CreateCachediSCSIVolumeOutput schema from Amazon Storage Gateway API
layout: schema
name: CreateCachediSCSIVolumeOutput
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: TargetARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-cachedi-scsi-volume-output-schema.json
slug: amazon-storage-gateway-create-cachedi-scsi-volume-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-cachedi-scsi-volume-output-schema.json\",\n  \"title\": \"CreateCachediSCSIVolumeOutput\",\n  \"description\": \"CreateCachediSCSIVolumeOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the configured volume.\"\n        }\n      ]\n    },\n    \"TargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume target, which includes the iSCSI name that initiators can use to connect to the target.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-cachedi-scsi-volume-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateCachediSCSIVolumeOutput
---
