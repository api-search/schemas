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
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SnapshotCopyGrant
---
