---
description: Returns the destination region and retention period that are configured for cross-region snapshot copy.
layout: schema
name: ClusterSnapshotCopyStatus
properties_list:
- description: ''
  name: DestinationRegion
  type: object
- description: ''
  name: RetentionPeriod
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
- description: ''
  name: SnapshotCopyGrantName
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-snapshot-copy-status-schema.json
slug: redshift-cluster-snapshot-copy-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationRegion\": {},\n    \"RetentionPeriod\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"SnapshotCopyGrantName\": {}\n  },\n  \"description\": \"Returns the destination region and retention period that are configured for cross-region snapshot copy.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-snapshot-copy-status-schema.json\",\n  \"title\": \"ClusterSnapshotCopyStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-snapshot-copy-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterSnapshotCopyStatus
---
