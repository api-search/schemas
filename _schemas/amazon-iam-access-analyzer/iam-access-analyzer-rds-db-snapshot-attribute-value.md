---
description: The name and values of a manual Amazon RDS DB snapshot attribute. Manual DB snapshot attributes are used to authorize other Amazon Web Services accounts to restore a manual DB snapshot.
layout: schema
name: RdsDbSnapshotAttributeValue
properties_list:
- description: ''
  name: accountIds
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-rds-db-snapshot-attribute-value-schema.json
slug: iam-access-analyzer-rds-db-snapshot-attribute-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-rds-db-snapshot-attribute-value-schema.json\",\n  \"title\": \"RdsDbSnapshotAttributeValue\",\n  \"description\": \"The name and values of a manual Amazon RDS DB snapshot attribute. Manual DB snapshot attributes are used to authorize other Amazon Web Services accounts to restore a manual DB snapshot.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RdsDbSnapshotAccountIdsList\"\n        },\n        {\n          \"description\": \"<p>The Amazon Web Services account IDs that have access to the manual Amazon RDS DB snapshot. If the value <code>all</code> is specified, then the Amazon RDS DB snapshot is public and can be copied or restored by all Amazon Web Services accounts.</p>\
  \ <ul> <li> <p>If the configuration is for an existing Amazon RDS DB snapshot and you do not specify the <code>accountIds</code> in <code>RdsDbSnapshotAttributeValue</code>, then the access preview uses the existing shared <code>accountIds</code> for the snapshot.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the specify the <code>accountIds</code> in <code>RdsDbSnapshotAttributeValue</code>, then the access preview considers the snapshot without any attributes.</p> </li> <li> <p>To propose deletion of an existing shared <code>accountIds</code>, you can specify an empty list for <code>accountIds</code> in the <code>RdsDbSnapshotAttributeValue</code>.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-rds-db-snapshot-attribute-value-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: RdsDbSnapshotAttributeValue
---
