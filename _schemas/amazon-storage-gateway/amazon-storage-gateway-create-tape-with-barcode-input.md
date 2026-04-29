---
description: CreateTapeWithBarcodeInput
layout: schema
name: CreateTapeWithBarcodeInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: TapeSizeInBytes
  type: object
- description: ''
  name: TapeBarcode
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
schema_file: json-schema/amazon-storage-gateway-create-tape-with-barcode-input-schema.json
slug: amazon-storage-gateway-create-tape-with-barcode-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-with-barcode-input-schema.json\",\n  \"title\": \"CreateTapeWithBarcodeInput\",\n  \"description\": \"CreateTapeWithBarcodeInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) that represents the gateway to associate the virtual tape with. Use the <a>ListGateways</a> operation to return a list of gateways for your account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"TapeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeSize\"\n        },\n        {\n          \"description\": \"<p>The size, in\
  \ bytes, of the virtual tape that you want to create.</p> <note> <p>The size must be aligned by gigabyte (1024*1024*1024 bytes).</p> </note>\"\n        }\n      ]\n    },\n    \"TapeBarcode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeBarcode\"\n        },\n        {\n          \"description\": \"<p>The barcode that you want to assign to the tape.</p> <note> <p>Barcodes cannot be reused. This includes barcodes used for tapes that have been deleted.</p> </note>\"\n        }\n      ]\n    },\n    \"KMSEncrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to use Amazon S3 server-side encryption with your own KMS key, or <code>false</code> to use a key managed by Amazon S3. Optional.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"KMSKey\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/KMSKey\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a symmetric customer master key (CMK) used for Amazon S3 server-side encryption. Storage Gateway does not support asymmetric CMKs. This value can only be set when <code>KMSEncrypted</code> is <code>true</code>. Optional.\"\n        }\n      ]\n    },\n    \"PoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolId\"\n        },\n        {\n          \"description\": \"The ID of the pool that you want to add your tape to for archiving. The tape in this pool is archived in the S3 storage class that is associated with the pool. When you use your backup application to eject the tape, the tape is archived directly into the storage class (S3 Glacier or S3 Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"Worm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\
  \n        },\n        {\n          \"description\": \"Set to <code>TRUE</code> if the tape you are creating is to be configured as a write-once-read-many (WORM) tape.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of up to 50 tags that can be assigned to a virtual tape that has a barcode. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"TapeSizeInBytes\",\n    \"TapeBarcode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-with-barcode-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateTapeWithBarcodeInput
---
