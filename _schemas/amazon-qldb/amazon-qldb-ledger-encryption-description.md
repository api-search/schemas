---
description: <p>Information about the encryption of data at rest in an Amazon QLDB ledger. This includes the current status, the key in Key Management Service (KMS), and when the key became inaccessible (in the case of an error).</p> <p>For more information, see <a href="https://docs.aws.amazon.com/qldb/latest/developerguide/encryption-at-rest.html">Encryption at rest</a> in the <i>Amazon QLDB Developer Guide</i>.</p>
layout: schema
name: LedgerEncryptionDescription
properties_list:
- description: ''
  name: KmsKeyArn
  type: object
- description: ''
  name: EncryptionStatus
  type: object
- description: ''
  name: InaccessibleKmsKeyDateTime
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-ledger-encryption-description-schema.json
slug: amazon-qldb-ledger-encryption-description
source_filename: amazon-qldb-ledger-encryption-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-ledger-encryption-description-schema.json\",\n  \"title\": \"LedgerEncryptionDescription\",\n  \"description\": \"<p>Information about the encryption of data at rest in an Amazon QLDB ledger. This includes the current status, the key in Key Management Service (KMS), and when the key became inaccessible (in the case of an error).</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/qldb/latest/developerguide/encryption-at-rest.html\\\">Encryption at rest</a> in the <i>Amazon QLDB Developer Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the customer managed KMS key that the\
  \ ledger uses for encryption at rest. If this parameter is undefined, the ledger uses an Amazon Web Services owned KMS key for encryption.\"\n        }\n      ]\n    },\n    \"EncryptionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionStatus\"\n        },\n        {\n          \"description\": \"<p>The current state of encryption at rest for the ledger. This can be one of the following values:</p> <ul> <li> <p> <code>ENABLED</code>: Encryption is fully enabled using the specified key.</p> </li> <li> <p> <code>UPDATING</code>: The ledger is actively processing the specified key change.</p> <p>Key changes in QLDB are asynchronous. The ledger is fully accessible without any performance impact while the key change is being processed. The amount of time it takes to update a key varies depending on the ledger size.</p> </li> <li> <p> <code>KMS_KEY_INACCESSIBLE</code>: The specified customer managed KMS key is not accessible, and the ledger is impaired.\
  \ Either the key was disabled or deleted, or the grants on the key were revoked. When a ledger is impaired, it is not accessible and does not accept any read or write requests.</p> <p>An impaired ledger automatically returns to an active state after you restore the grants on the key, or re-enable the key that was disabled. However, deleting a customer managed KMS key is irreversible. After a key is deleted, you can no longer access the ledgers that are protected with that key, and the data becomes unrecoverable permanently.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"InaccessibleKmsKeyDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The date and time, in epoch time format, when the KMS key first became inaccessible, in the case of an error. (Epoch time format is the number of seconds that have elapsed since 12:00:00 AM January 1, 1970 UTC.)</p> <p>This parameter is undefined\
  \ if the KMS key is accessible.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KmsKeyArn\",\n    \"EncryptionStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-ledger-encryption-description-schema.json
tags:
- Blockchain
- Database
- Ledger
title: LedgerEncryptionDescription
---
