---
description: AssignTapePoolInput schema from Amazon Storage Gateway API
layout: schema
name: AssignTapePoolInput
properties_list:
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: PoolId
  type: object
- description: ''
  name: BypassGovernanceRetention
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-assign-tape-pool-input-schema.json
slug: amazon-storage-gateway-assign-tape-pool-input
source_filename: amazon-storage-gateway-assign-tape-pool-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-assign-tape-pool-input-schema.json\",\n  \"title\": \"AssignTapePoolInput\",\n  \"description\": \"AssignTapePoolInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) of the virtual tape that you want to add to the tape pool.\"\n        }\n      ]\n    },\n    \"PoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolId\"\n        },\n        {\n          \"description\": \"The ID of the pool that you want to add your tape to for archiving. The tape in this pool is archived in the S3 storage class that is associated\
  \ with the pool. When you use your backup application to eject the tape, the tape is archived directly into the storage class (S3 Glacier or S3 Glacier Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"BypassGovernanceRetention\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"<p>Set permissions to bypass governance retention. If the lock type of the archived tape is <code>Governance</code>, the tape's archived age is not older than <code>RetentionLockInDays</code>, and the user does not already have <code>BypassGovernanceRetention</code>, setting this to TRUE enables the user to bypass the retention lock. This parameter is set to true by default for calls from the console.</p> <p>Valid values: <code>TRUE</code> | <code>FALSE</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TapeARN\",\n    \"PoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-assign-tape-pool-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AssignTapePoolInput
---
