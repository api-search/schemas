---
description: Describes a recovery point.
layout: schema
name: TapeRecoveryPointInfo
properties_list:
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: TapeRecoveryPointTime
  type: object
- description: ''
  name: TapeSizeInBytes
  type: object
- description: ''
  name: TapeStatus
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-tape-recovery-point-info-schema.json
slug: amazon-storage-gateway-tape-recovery-point-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-recovery-point-info-schema.json\",\n  \"title\": \"TapeRecoveryPointInfo\",\n  \"description\": \"Describes a recovery point.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape.\"\n        }\n      ]\n    },\n    \"TapeRecoveryPointTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"<p>The time when the point-in-time view of the virtual tape was replicated for later recovery.</p> <p>The default timestamp format of the tape recovery point time is in the ISO8601 extended YYYY-MM-DD'T'HH:MM:SS'Z'\
  \ format.</p>\"\n        }\n      ]\n    },\n    \"TapeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeSize\"\n        },\n        {\n          \"description\": \"The size, in bytes, of the virtual tapes to recover.\"\n        }\n      ]\n    },\n    \"TapeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeRecoveryPointStatus\"\n        },\n        {\n          \"description\": \"The status of the virtual tapes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-recovery-point-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: TapeRecoveryPointInfo
---
