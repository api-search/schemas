---
description: RevokeSnapshotAccessResult schema from Amazon Redshift
layout: schema
name: RevokeSnapshotAccessResult
properties_list:
- description: Describes a snapshot.
  name: Snapshot
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-revoke-snapshot-access-result-schema.json
slug: redshift-revoke-snapshot-access-result
source_filename: redshift-revoke-snapshot-access-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Snapshot\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"SnapshotIdentifier\": {},\n        \"ClusterIdentifier\": {},\n        \"SnapshotCreateTime\": {},\n        \"Status\": {},\n        \"Port\": {},\n        \"AvailabilityZone\": {},\n        \"ClusterCreateTime\": {},\n        \"MasterUsername\": {},\n        \"ClusterVersion\": {},\n        \"EngineFullVersion\": {},\n        \"SnapshotType\": {},\n        \"NodeType\": {},\n        \"NumberOfNodes\": {},\n        \"DBName\": {},\n        \"VpcId\": {},\n        \"Encrypted\": {},\n        \"KmsKeyId\": {},\n        \"EncryptedWithHSM\": {},\n        \"AccountsWithRestoreAccess\": {},\n        \"OwnerAccount\": {},\n        \"TotalBackupSizeInMegaBytes\": {},\n        \"ActualIncrementalBackupSizeInMegaBytes\": {},\n        \"BackupProgressInMegaBytes\": {},\n        \"CurrentBackupRateInMegaBytesPerSecond\": {},\n        \"EstimatedSecondsToCompletion\"\
  : {},\n        \"ElapsedTimeInSeconds\": {},\n        \"SourceRegion\": {},\n        \"Tags\": {},\n        \"RestorableNodeTypes\": {},\n        \"EnhancedVpcRouting\": {},\n        \"MaintenanceTrackName\": {},\n        \"ManualSnapshotRetentionPeriod\": {},\n        \"ManualSnapshotRemainingDays\": {},\n        \"SnapshotRetentionStartTime\": {}\n      },\n      \"description\": \"Describes a snapshot.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-revoke-snapshot-access-result-schema.json\",\n  \"title\": \"RevokeSnapshotAccessResult\",\n  \"description\": \"RevokeSnapshotAccessResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-revoke-snapshot-access-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RevokeSnapshotAccessResult
---
