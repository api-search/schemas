---
description: CreateTapesInput
layout: schema
name: CreateTapesInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: TapeSizeInBytes
  type: object
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: NumTapesToCreate
  type: object
- description: ''
  name: TapeBarcodePrefix
  type: object
- description: ''
  name: KMSEncrypted
  type: object
- description: ''
  name: KMSKey
  type: object
- description: ''
  name: PoolId
  type: object
- description: ''
  name: Worm
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-tapes-input-schema.json
slug: amazon-storage-gateway-create-tapes-input
source_filename: amazon-storage-gateway-create-tapes-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tapes-input-schema.json\",\n  \"title\": \"CreateTapesInput\",\n  \"description\": \"CreateTapesInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) that represents the gateway to associate the virtual tapes with. Use the <a>ListGateways</a> operation to return a list of gateways for your account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"TapeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeSize\"\n        },\n        {\n          \"description\": \"<p>The size, in bytes, of the virtual tapes that\
  \ you want to create.</p> <note> <p>The size must be aligned by gigabyte (1024*1024*1024 bytes).</p> </note>\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"<p>A unique identifier that you use to retry a request. If you retry a request, use the same <code>ClientToken</code> you specified in the initial request.</p> <note> <p>Using the same <code>ClientToken</code> prevents creating the tape multiple times.</p> </note>\"\n        }\n      ]\n    },\n    \"NumTapesToCreate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumTapesToCreate\"\n        },\n        {\n          \"description\": \"The number of virtual tapes that you want to create.\"\n        }\n      ]\n    },\n    \"TapeBarcodePrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeBarcodePrefix\"\n        },\n  \
  \      {\n          \"description\": \"<p>A prefix that you append to the barcode of the virtual tape you are creating. This prefix makes the barcode unique.</p> <note> <p>The prefix must be 1-4 characters in length and must be one of the uppercase letters from A to Z.</p> </note>\"\n        }\n      ]\n    },\n    \"KMSEncrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to use Amazon S3 server-side encryption with your own KMS key, or <code>false</code> to use a key managed by Amazon S3. Optional.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"KMSKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KMSKey\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a symmetric customer master key (CMK) used for Amazon S3 server-side encryption. Storage\
  \ Gateway does not support asymmetric CMKs. This value can only be set when <code>KMSEncrypted</code> is <code>true</code>. Optional.\"\n        }\n      ]\n    },\n    \"PoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolId\"\n        },\n        {\n          \"description\": \"The ID of the pool that you want to add your tape to for archiving. The tape in this pool is archived in the S3 storage class that is associated with the pool. When you use your backup application to eject the tape, the tape is archived directly into the storage class (S3 Glacier or S3 Glacier Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"Worm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Set to <code>TRUE</code> if the tape you are creating is to be configured as a write-once-read-many (WORM) tape.\"\n        }\n      ]\n    },\n    \"Tags\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of up to 50 tags that can be assigned to a virtual tape. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"TapeSizeInBytes\",\n    \"ClientToken\",\n    \"NumTapesToCreate\",\n    \"TapeBarcodePrefix\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tapes-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateTapesInput
---
