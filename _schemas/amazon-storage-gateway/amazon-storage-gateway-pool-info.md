---
description: Describes a custom tape pool.
layout: schema
name: PoolInfo
properties_list:
- description: ''
  name: PoolARN
  type: object
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
  name: PoolStatus
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-pool-info-schema.json
slug: amazon-storage-gateway-pool-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-pool-info-schema.json\",\n  \"title\": \"PoolInfo\",\n  \"description\": \"Describes a custom tape pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PoolARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom tape pool. Use the <a>ListTapePools</a> operation to return a list of custom tape pools for your account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"PoolName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolName\"\n        },\n        {\n          \"description\": \"The name of the custom tape pool. <code>PoolName</code> can use all ASCII characters, except '/' and\
  \ '\\\\'.\"\n        }\n      ]\n    },\n    \"StorageClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeStorageClass\"\n        },\n        {\n          \"description\": \"The storage class that is associated with the custom pool. When you use your backup application to eject the tape, the tape is archived directly into the storage class (S3 Glacier or S3 Glacier Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"RetentionLockType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionLockType\"\n        },\n        {\n          \"description\": \"Tape retention lock type, which can be configured in two modes. When configured in governance mode, Amazon Web Services accounts with specific IAM permissions are authorized to remove the tape retention lock from archived virtual tapes. When configured in compliance mode, the tape retention lock cannot be removed by any user, including the\
  \ root Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"RetentionLockTimeInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetentionLockTimeInDays\"\n        },\n        {\n          \"description\": \"Tape retention lock time is set in days. Tape retention lock can be enabled for up to 100 years (36,500 days).\"\n        }\n      ]\n    },\n    \"PoolStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolStatus\"\n        },\n        {\n          \"description\": \"Status of the custom tape pool. Pool can be <code>ACTIVE</code> or <code>DELETED</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-pool-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: PoolInfo
---
