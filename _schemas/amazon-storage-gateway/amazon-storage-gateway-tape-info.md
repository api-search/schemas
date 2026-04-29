---
description: Describes a virtual tape.
layout: schema
name: TapeInfo
properties_list:
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: TapeBarcode
  type: object
- description: ''
  name: TapeSizeInBytes
  type: object
- description: ''
  name: TapeStatus
  type: object
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: PoolId
  type: object
- description: ''
  name: RetentionStartDate
  type: object
- description: ''
  name: PoolEntryDate
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-tape-info-schema.json
slug: amazon-storage-gateway-tape-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-info-schema.json\",\n  \"title\": \"TapeInfo\",\n  \"description\": \"Describes a virtual tape.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a virtual tape.\"\n        }\n      ]\n    },\n    \"TapeBarcode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeBarcode\"\n        },\n        {\n          \"description\": \"The barcode that identifies a specific virtual tape.\"\n        }\n      ]\n    },\n    \"TapeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeSize\"\n        },\n        {\n       \
  \   \"description\": \"The size, in bytes, of a virtual tape.\"\n        }\n      ]\n    },\n    \"TapeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeStatus\"\n        },\n        {\n          \"description\": \"The status of the tape.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the gateway. Use the <a>ListGateways</a> operation to return a list of gateways for your account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"PoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolId\"\n        },\n        {\n          \"description\": \"The ID of the pool that you want to add your tape to for archiving. The tape in this pool is archived in the S3 storage class that is associated with the pool. When you use your\
  \ backup application to eject the tape, the tape is archived directly into the storage class (S3 Glacier or S3 Glacier Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"RetentionStartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"The date that the tape became subject to tape retention lock.\"\n        }\n      ]\n    },\n    \"PoolEntryDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"The date that the tape entered the custom tape pool with tape retention lock enabled.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: TapeInfo
---
