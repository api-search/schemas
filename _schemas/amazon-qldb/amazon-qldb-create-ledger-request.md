---
description: CreateLedgerRequest schema from Amazon QLDB API
layout: schema
name: CreateLedgerRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: PermissionsMode
  type: object
- description: ''
  name: DeletionProtection
  type: object
- description: ''
  name: KmsKey
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-create-ledger-request-schema.json
slug: amazon-qldb-create-ledger-request
source_filename: amazon-qldb-create-ledger-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-create-ledger-request-schema.json\",\n  \"title\": \"CreateLedgerRequest\",\n  \"description\": \"CreateLedgerRequest schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerName\"\n        },\n        {\n          \"description\": \"<p>The name of the ledger that you want to create. The name must be unique among all of the ledgers in your Amazon Web Services account in the current Region.</p> <p>Naming constraints for ledger names are defined in <a href=\\\"https://docs.aws.amazon.com/qldb/latest/developerguide/limits.html#limits.naming\\\">Quotas in Amazon QLDB</a> in the <i>Amazon QLDB Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The key-value pairs to add as tags to the ledger that you want to create. Tag keys are case sensitive. Tag values are case sensitive and can be null.\"\n        }\n      ]\n    },\n    \"PermissionsMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionsMode\"\n        },\n        {\n          \"description\": \"<p>The permissions mode to assign to the ledger that you want to create. This parameter can have one of the following values:</p> <ul> <li> <p> <code>ALLOW_ALL</code>: A legacy permissions mode that enables access control with API-level granularity for ledgers.</p> <p>This mode allows users who have the <code>SendCommand</code> API permission for this ledger to run all PartiQL commands (hence, <code>ALLOW_ALL</code>) on any tables in the specified ledger. This mode disregards any table-level or command-level IAM permissions\
  \ policies that you create for the ledger.</p> </li> <li> <p> <code>STANDARD</code>: (<i>Recommended</i>) A permissions mode that enables access control with finer granularity for ledgers, tables, and PartiQL commands.</p> <p>By default, this mode denies all user requests to run any PartiQL commands on any tables in this ledger. To allow PartiQL commands to run, you must create IAM permissions policies for specific table resources and PartiQL actions, in addition to the <code>SendCommand</code> API permission for the ledger. For information, see <a href=\\\"https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started-standard-mode.html\\\">Getting started with the standard permissions mode</a> in the <i>Amazon QLDB Developer Guide</i>.</p> </li> </ul> <note> <p>We strongly recommend using the <code>STANDARD</code> permissions mode to maximize the security of your ledger data.</p> </note>\"\n        }\n      ]\n    },\n    \"DeletionProtection\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/DeletionProtection\"\n        },\n        {\n          \"description\": \"<p>The flag that prevents a ledger from being deleted by any user. If not provided on ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>\"\n        }\n      ]\n    },\n    \"KmsKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKey\"\n        },\n        {\n          \"description\": \"<p>The key in Key Management Service (KMS) to use for encryption of data at rest in the ledger. For more information, see <a href=\\\"https://docs.aws.amazon.com/qldb/latest/developerguide/encryption-at-rest.html\\\">Encryption at rest</a> in the <i>Amazon QLDB Developer Guide</i>.</p> <p>Use one of the following options\
  \ to specify this parameter:</p> <ul> <li> <p> <code>AWS_OWNED_KMS_KEY</code>: Use an KMS key that is owned and managed by Amazon Web Services on your behalf.</p> </li> <li> <p> <b>Undefined</b>: By default, use an Amazon Web Services owned KMS key.</p> </li> <li> <p> <b>A valid symmetric customer managed KMS key</b>: Use the specified KMS key in your account that you create, own, and manage.</p> <p>Amazon QLDB does not support asymmetric keys. For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html\\\">Using symmetric and asymmetric keys</a> in the <i>Key Management Service Developer Guide</i>.</p> </li> </ul> <p>To specify a customer managed KMS key, you can use its key ID, Amazon Resource Name (ARN), alias name, or alias ARN. When using an alias name, prefix it with <code>\\\"alias/\\\"</code>. To specify a key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul>\
  \ <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id\\\">Key identifiers (KeyId)</a> in the <i>Key Management Service Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"PermissionsMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-create-ledger-request-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: CreateLedgerRequest
---
