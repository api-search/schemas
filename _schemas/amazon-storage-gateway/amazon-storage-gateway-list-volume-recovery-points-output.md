---
description: ListVolumeRecoveryPointsOutput schema from Amazon Storage Gateway API
layout: schema
name: ListVolumeRecoveryPointsOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: VolumeRecoveryPointInfos
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-volume-recovery-points-output-schema.json
slug: amazon-storage-gateway-list-volume-recovery-points-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volume-recovery-points-output-schema.json\",\n  \"title\": \"ListVolumeRecoveryPointsOutput\",\n  \"description\": \"ListVolumeRecoveryPointsOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"VolumeRecoveryPointInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeRecoveryPointInfos\"\n        },\n        {\n          \"description\": \"An array of <a>VolumeRecoveryPointInfo</a> objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volume-recovery-points-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListVolumeRecoveryPointsOutput
---
