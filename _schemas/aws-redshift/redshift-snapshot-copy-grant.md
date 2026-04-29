---
description: <p>The snapshot copy grant that grants Amazon Redshift permission to encrypt copied snapshots with the specified encrypted symmetric key from Amazon Web Services KMS in the destination region.</p> <p> For more information about managing snapshot copy grants, go to <a href="https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-db-encryption.html">Amazon Redshift Database Encryption</a> in the <i>Amazon Redshift Cluster Management Guide</i>. </p>
layout: schema
name: SnapshotCopyGrant
properties_list:
- description: ''
  name: SnapshotCopyGrantName
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-snapshot-copy-grant-schema.json
slug: redshift-snapshot-copy-grant
source_filename: redshift-snapshot-copy-grant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotCopyGrantName\": {},\n    \"KmsKeyId\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"<p>The snapshot copy grant that grants Amazon Redshift permission to encrypt copied snapshots with the specified encrypted symmetric key from Amazon Web Services KMS in the destination region.</p> <p> For more information about managing snapshot copy grants, go to <a href=\\\"https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-db-encryption.html\\\">Amazon Redshift Database Encryption</a> in the <i>Amazon Redshift Cluster Management Guide</i>. </p>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-copy-grant-schema.json\",\n  \"title\": \"SnapshotCopyGrant\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-copy-grant-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SnapshotCopyGrant
---
