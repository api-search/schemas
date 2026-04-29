---
description: CreateTapePoolInput schema from Amazon Storage Gateway API
layout: schema
name: CreateTapePoolInput
properties_list:
- description: ''
  name: PoolName
  type: object
- description: ''
  name: StorageClass
  type: object
- description: ''
  name: RetentionLockType
  type: object
- description: ''
  name: RetentionLockTimeInDays
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-tape-pool-input-schema.json
slug: amazon-storage-gateway-create-tape-pool-input
source_filename: amazon-storage-gateway-create-tape-pool-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-pool-input-schema.json\",\n  \"title\": \"CreateTapePoolInput\",\n  \"description\": \"CreateTapePoolInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PoolName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolName\"\n        },\n        {\n          \"description\": \"The name of the new custom tape pool.\"\n        }\n      ]\n    },\n    \"StorageClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeStorageClass\"\n        },\n        {\n          \"description\": \"The storage class that is associated with the new custom pool. When you use your backup application to eject the tape, the tape is archived directly into the storage class (S3\
  \ Glacier or S3 Glacier Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"RetentionLockType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionLockType\"\n        },\n        {\n          \"description\": \"Tape retention lock can be configured in two modes. When configured in governance mode, Amazon Web Services accounts with specific IAM permissions are authorized to remove the tape retention lock from archived virtual tapes. When configured in compliance mode, the tape retention lock cannot be removed by any user, including the root Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"RetentionLockTimeInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionLockTimeInDays\"\n        },\n        {\n          \"description\": \"Tape retention lock time is set in days. Tape retention lock can be enabled for up to 100 years (36,500 days).\"\n        }\n      ]\n    },\n\
  \    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of up to 50 tags that can be assigned to tape pool. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PoolName\",\n    \"StorageClass\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-pool-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateTapePoolInput
---
