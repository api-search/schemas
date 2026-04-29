---
description: CreateLedgerResponse schema from Amazon QLDB API
layout: schema
name: CreateLedgerResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: CreationDateTime
  type: object
- description: ''
  name: PermissionsMode
  type: object
- description: ''
  name: DeletionProtection
  type: object
- description: ''
  name: KmsKeyArn
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-create-ledger-response-schema.json
slug: amazon-qldb-create-ledger-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-create-ledger-response-schema.json\",\n  \"title\": \"CreateLedgerResponse\",\n  \"description\": \"CreateLedgerResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerName\"\n        },\n        {\n          \"description\": \"The name of the ledger.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the ledger.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerState\"\n        },\n        {\n          \"description\": \"The current\
  \ status of the ledger.\"\n        }\n      ]\n    },\n    \"CreationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time, in epoch time format, when the ledger was created. (Epoch time format is the number of seconds elapsed since 12:00:00 AM January 1, 1970 UTC.)\"\n        }\n      ]\n    },\n    \"PermissionsMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionsMode\"\n        },\n        {\n          \"description\": \"The permissions mode of the ledger that you created.\"\n        }\n      ]\n    },\n    \"DeletionProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeletionProtection\"\n        },\n        {\n          \"description\": \"<p>The flag that prevents a ledger from being deleted by any user. If not provided on ledger creation, this feature is enabled (<code>true</code>) by\
  \ default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the customer managed KMS key that the ledger uses for encryption at rest. If this parameter is undefined, the ledger uses an Amazon Web Services owned KMS key for encryption.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-create-ledger-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: CreateLedgerResponse
---
