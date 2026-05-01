---
description: The proposed access control configuration for an Amazon RDS DB cluster snapshot. You can propose a configuration for a new Amazon RDS DB cluster snapshot or an Amazon RDS DB cluster snapshot that you own by specifying the <code>RdsDbClusterSnapshotAttributeValue</code> and optional KMS encryption key. For more information, see <a href="https://docs.aws.amazon.com/AmazonRDS/latest/APIReference/API_ModifyDBClusterSnapshotAttribute.html">ModifyDBClusterSnapshotAttribute</a>.
layout: schema
name: RdsDbClusterSnapshotConfiguration
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: kmsKeyId
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-rds-db-cluster-snapshot-configuration-schema.json
slug: iam-access-analyzer-rds-db-cluster-snapshot-configuration
source_filename: iam-access-analyzer-rds-db-cluster-snapshot-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-rds-db-cluster-snapshot-configuration-schema.json\",\n  \"title\": \"RdsDbClusterSnapshotConfiguration\",\n  \"description\": \"The proposed access control configuration for an Amazon RDS DB cluster snapshot. You can propose a configuration for a new Amazon RDS DB cluster snapshot or an Amazon RDS DB cluster snapshot that you own by specifying the <code>RdsDbClusterSnapshotAttributeValue</code> and optional KMS encryption key. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonRDS/latest/APIReference/API_ModifyDBClusterSnapshotAttribute.html\\\">ModifyDBClusterSnapshotAttribute</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RdsDbClusterSnapshotAttributesMap\"\
  \n        },\n        {\n          \"description\": \"The names and values of manual DB cluster snapshot attributes. Manual DB cluster snapshot attributes are used to authorize other Amazon Web Services accounts to restore a manual DB cluster snapshot. The only valid value for <code>AttributeName</code> for the attribute map is <code>restore</code> \"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RdsDbClusterSnapshotKmsKeyId\"\n        },\n        {\n          \"description\": \"<p>The KMS key identifier for an encrypted Amazon RDS DB cluster snapshot. The KMS key identifier is the key ARN, key ID, alias ARN, or alias name for the KMS key.</p> <ul> <li> <p>If the configuration is for an existing Amazon RDS DB cluster snapshot and you do not specify the <code>kmsKeyId</code>, or you specify an empty string, then the access preview uses the existing <code>kmsKeyId</code> of the snapshot.</p> </li> <li> <p>If the\
  \ access preview is for a new resource and you do not specify the specify the <code>kmsKeyId</code>, then the access preview considers the snapshot as unencrypted.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-rds-db-cluster-snapshot-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: RdsDbClusterSnapshotConfiguration
---
