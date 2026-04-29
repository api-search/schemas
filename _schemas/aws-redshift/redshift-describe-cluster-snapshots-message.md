---
description: <p/>
layout: schema
name: DescribeClusterSnapshotsMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: SnapshotArn
  type: object
- description: ''
  name: SnapshotType
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: MaxRecords
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: OwnerAccount
  type: object
- description: ''
  name: TagKeys
  type: object
- description: ''
  name: TagValues
  type: object
- description: ''
  name: ClusterExists
  type: object
- description: ''
  name: SortingEntities
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-describe-cluster-snapshots-message-schema.json
slug: redshift-describe-cluster-snapshots-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"SnapshotIdentifier\": {},\n    \"SnapshotArn\": {},\n    \"SnapshotType\": {},\n    \"StartTime\": {},\n    \"EndTime\": {},\n    \"MaxRecords\": {},\n    \"Marker\": {},\n    \"OwnerAccount\": {},\n    \"TagKeys\": {},\n    \"TagValues\": {},\n    \"ClusterExists\": {},\n    \"SortingEntities\": {}\n  },\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-cluster-snapshots-message-schema.json\",\n  \"title\": \"DescribeClusterSnapshotsMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-cluster-snapshots-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DescribeClusterSnapshotsMessage
---
