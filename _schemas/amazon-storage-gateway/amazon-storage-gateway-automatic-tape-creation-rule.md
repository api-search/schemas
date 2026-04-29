---
description: An automatic tape creation policy consists of automatic tape creation rules where each rule defines when and how to create new tapes. For more information about automatic tape creation, see <a href="https://docs.aws.amazon.com/storagegateway/latest/userguide/GettingStartedCreateTapes.html#CreateTapesAutomatically">Creating Tapes Automatically</a>.
layout: schema
name: AutomaticTapeCreationRule
properties_list:
- description: ''
  name: TapeBarcodePrefix
  type: object
- description: ''
  name: PoolId
  type: object
- description: ''
  name: TapeSizeInBytes
  type: object
- description: ''
  name: MinimumNumTapes
  type: object
- description: ''
  name: Worm
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-automatic-tape-creation-rule-schema.json
slug: amazon-storage-gateway-automatic-tape-creation-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-automatic-tape-creation-rule-schema.json\",\n  \"title\": \"AutomaticTapeCreationRule\",\n  \"description\": \"An automatic tape creation policy consists of automatic tape creation rules where each rule defines when and how to create new tapes. For more information about automatic tape creation, see <a href=\\\"https://docs.aws.amazon.com/storagegateway/latest/userguide/GettingStartedCreateTapes.html#CreateTapesAutomatically\\\">Creating Tapes Automatically</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeBarcodePrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeBarcodePrefix\"\n        },\n        {\n          \"description\": \"<p>A prefix that you append to the barcode of the virtual tape that you are creating. This\
  \ prefix makes the barcode unique.</p> <note> <p>The prefix must be 1-4 characters in length and must be one of the uppercase letters from A to Z.</p> </note>\"\n        }\n      ]\n    },\n    \"PoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolId\"\n        },\n        {\n          \"description\": \"The ID of the pool that you want to add your tape to for archiving. The tape in this pool is archived in the Amazon S3 storage class that is associated with the pool. When you use your backup application to eject the tape, the tape is archived directly into the storage class (S3 Glacier or S3 Glacier Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"TapeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeSize\"\n        },\n        {\n          \"description\": \"The size, in bytes, of the virtual tape capacity.\"\n        }\n      ]\n    },\n    \"MinimumNumTapes\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinimumNumTapes\"\n        },\n        {\n          \"description\": \"The minimum number of available virtual tapes that the gateway maintains at all times. If the number of tapes on the gateway goes below this value, the gateway creates as many new tapes as are needed to have <code>MinimumNumTapes</code> on the gateway. For more information about automatic tape creation, see <a href=\\\"https://docs.aws.amazon.com/storagegateway/latest/userguide/GettingStartedCreateTapes.html#CreateTapesAutomatically\\\">Creating Tapes Automatically</a>.\"\n        }\n      ]\n    },\n    \"Worm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Set to <code>true</code> to indicate that tapes are to be archived as write-once-read-many (WORM). Set to <code>false</code> when WORM is not enabled for tapes.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"TapeBarcodePrefix\",\n    \"PoolId\",\n    \"TapeSizeInBytes\",\n    \"MinimumNumTapes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-automatic-tape-creation-rule-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AutomaticTapeCreationRule
---
