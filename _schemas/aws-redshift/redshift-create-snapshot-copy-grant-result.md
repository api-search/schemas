---
description: CreateSnapshotCopyGrantResult schema from Amazon Redshift
layout: schema
name: CreateSnapshotCopyGrantResult
properties_list:
- description: <p>The snapshot copy grant that grants Amazon Redshift permission to encrypt copied snapshots with the specified encrypted symmetric key from Amazon Web Services KMS in the destination region.</p> <p>
  name: SnapshotCopyGrant
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-snapshot-copy-grant-result-schema.json
slug: redshift-create-snapshot-copy-grant-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotCopyGrant\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"SnapshotCopyGrantName\": {},\n        \"KmsKeyId\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"<p>The snapshot copy grant that grants Amazon Redshift permission to encrypt copied snapshots with the specified encrypted symmetric key from Amazon Web Services KMS in the destination region.</p> <p> For more information about managing snapshot copy grants, go to <a href=\\\"https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-db-encryption.html\\\">Amazon Redshift Database Encryption</a> in the <i>Amazon Redshift Cluster Management Guide</i>. </p>\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-snapshot-copy-grant-result-schema.json\",\n  \"title\": \"CreateSnapshotCopyGrantResult\"\
  ,\n  \"description\": \"CreateSnapshotCopyGrantResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-snapshot-copy-grant-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateSnapshotCopyGrantResult
---
