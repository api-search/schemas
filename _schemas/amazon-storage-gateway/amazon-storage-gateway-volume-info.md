---
description: Describes a storage volume object.
layout: schema
name: VolumeInfo
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: VolumeId
  type: object
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: GatewayId
  type: object
- description: ''
  name: VolumeType
  type: object
- description: ''
  name: VolumeSizeInBytes
  type: object
- description: ''
  name: VolumeAttachmentStatus
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-volume-info-schema.json
slug: amazon-storage-gateway-volume-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-volume-info-schema.json\",\n  \"title\": \"VolumeInfo\",\n  \"description\": \"Describes a storage volume object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) for the storage volume. For example, the following is a valid ARN:</p> <p> <code>arn:aws:storagegateway:us-east-2:111122223333:gateway/sgw-12A3456B/volume/vol-1122AABB</code> </p> <p>Valid Values: 50 to 500 lowercase letters, numbers, periods (.), and hyphens (-).</p>\"\n        }\n      ]\n    },\n    \"VolumeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeId\"\n        },\n    \
  \    {\n          \"description\": \"<p>The unique identifier assigned to the volume. This ID becomes part of the volume Amazon Resource Name (ARN), which you use as input for other operations.</p> <p>Valid Values: 50 to 500 lowercase letters, numbers, periods (.), and hyphens (-).</p>\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"GatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayId\"\n        },\n        {\n          \"description\": \"<p>The unique identifier assigned to your gateway during activation. This ID becomes part of the gateway Amazon Resource Name (ARN), which you use as input for other operations.</p> <p>Valid Values: 50 to 500 lowercase letters, numbers, periods (.), and hyphens (-).</p>\"\n        }\n      ]\n    },\n    \"VolumeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeType\"\n        },\n        {\n\
  \          \"description\": \"One of the VolumeType enumeration values describing the type of the volume.\"\n        }\n      ]\n    },\n    \"VolumeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"<p>The size of the volume in bytes.</p> <p>Valid Values: 50 to 500 lowercase letters, numbers, periods (.), and hyphens (-).</p>\"\n        }\n      ]\n    },\n    \"VolumeAttachmentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeAttachmentStatus\"\n        },\n        {\n          \"description\": \"One of the VolumeStatus values that indicates the state of the storage volume.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-volume-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: VolumeInfo
---
