---
description: The proposed access control configuration for an Amazon EBS volume snapshot. You can propose a configuration for a new Amazon EBS volume snapshot or an Amazon EBS volume snapshot that you own by specifying the user IDs, groups, and optional KMS encryption key. For more information, see <a href="https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_ModifySnapshotAttribute.html">ModifySnapshotAttribute</a>.
layout: schema
name: EbsSnapshotConfiguration
properties_list:
- description: ''
  name: userIds
  type: object
- description: ''
  name: groups
  type: object
- description: ''
  name: kmsKeyId
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-ebs-snapshot-configuration-schema.json
slug: iam-access-analyzer-ebs-snapshot-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-ebs-snapshot-configuration-schema.json\",\n  \"title\": \"EbsSnapshotConfiguration\",\n  \"description\": \"The proposed access control configuration for an Amazon EBS volume snapshot. You can propose a configuration for a new Amazon EBS volume snapshot or an Amazon EBS volume snapshot that you own by specifying the user IDs, groups, and optional KMS encryption key. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_ModifySnapshotAttribute.html\\\">ModifySnapshotAttribute</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsUserIdList\"\n        },\n        {\n          \"description\": \"<p>The IDs of the Amazon Web Services accounts\
  \ that have access to the Amazon EBS volume snapshot.</p> <ul> <li> <p>If the configuration is for an existing Amazon EBS volume snapshot and you do not specify the <code>userIds</code>, then the access preview uses the existing shared <code>userIds</code> for the snapshot.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the <code>userIds</code>, then the access preview considers the snapshot without any <code>userIds</code>.</p> </li> <li> <p>To propose deletion of existing shared <code>accountIds</code>, you can specify an empty list for <code>userIds</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsGroupList\"\n        },\n        {\n          \"description\": \"<p>The groups that have access to the Amazon EBS volume snapshot. If the value <code>all</code> is specified, then the Amazon EBS volume snapshot is public.</p> <ul> <li> <p>If the configuration\
  \ is for an existing Amazon EBS volume snapshot and you do not specify the <code>groups</code>, then the access preview uses the existing shared <code>groups</code> for the snapshot.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the <code>groups</code>, then the access preview considers the snapshot without any <code>groups</code>.</p> </li> <li> <p>To propose deletion of existing shared <code>groups</code>, you can specify an empty list for <code>groups</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsSnapshotDataEncryptionKeyId\"\n        },\n        {\n          \"description\": \"<p>The KMS key identifier for an encrypted Amazon EBS volume snapshot. The KMS key identifier is the key ARN, key ID, alias ARN, or alias name for the KMS key.</p> <ul> <li> <p>If the configuration is for an existing Amazon EBS volume snapshot and you do not specify\
  \ the <code>kmsKeyId</code>, or you specify an empty string, then the access preview uses the existing <code>kmsKeyId</code> of the snapshot.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the <code>kmsKeyId</code>, the access preview considers the snapshot as unencrypted.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-ebs-snapshot-configuration-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: EbsSnapshotConfiguration
---
