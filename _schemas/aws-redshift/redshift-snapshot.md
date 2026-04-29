---
description: Describes a snapshot.
layout: schema
name: Snapshot
properties_list:
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: SnapshotCreateTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: ClusterCreateTime
  type: object
- description: ''
  name: MasterUsername
  type: object
- description: ''
  name: ClusterVersion
  type: object
- description: ''
  name: EngineFullVersion
  type: object
- description: ''
  name: SnapshotType
  type: object
- description: ''
  name: NodeType
  type: object
- description: ''
  name: NumberOfNodes
  type: object
- description: ''
  name: DBName
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: Encrypted
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: EncryptedWithHSM
  type: object
- description: ''
  name: AccountsWithRestoreAccess
  type: object
- description: ''
  name: OwnerAccount
  type: object
- description: ''
  name: TotalBackupSizeInMegaBytes
  type: object
- description: ''
  name: ActualIncrementalBackupSizeInMegaBytes
  type: object
- description: ''
  name: BackupProgressInMegaBytes
  type: object
- description: ''
  name: CurrentBackupRateInMegaBytesPerSecond
  type: object
- description: ''
  name: EstimatedSecondsToCompletion
  type: object
- description: ''
  name: ElapsedTimeInSeconds
  type: object
- description: ''
  name: SourceRegion
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: RestorableNodeTypes
  type: object
- description: ''
  name: EnhancedVpcRouting
  type: object
- description: ''
  name: MaintenanceTrackName
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
- description: ''
  name: ManualSnapshotRemainingDays
  type: object
- description: ''
  name: SnapshotRetentionStartTime
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-snapshot-schema.json
slug: redshift-snapshot
source_filename: redshift-snapshot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotIdentifier\": {},\n    \"ClusterIdentifier\": {},\n    \"SnapshotCreateTime\": {},\n    \"Status\": {},\n    \"Port\": {},\n    \"AvailabilityZone\": {},\n    \"ClusterCreateTime\": {},\n    \"MasterUsername\": {},\n    \"ClusterVersion\": {},\n    \"EngineFullVersion\": {},\n    \"SnapshotType\": {},\n    \"NodeType\": {},\n    \"NumberOfNodes\": {},\n    \"DBName\": {},\n    \"VpcId\": {},\n    \"Encrypted\": {},\n    \"KmsKeyId\": {},\n    \"EncryptedWithHSM\": {},\n    \"AccountsWithRestoreAccess\": {},\n    \"OwnerAccount\": {},\n    \"TotalBackupSizeInMegaBytes\": {},\n    \"ActualIncrementalBackupSizeInMegaBytes\": {},\n    \"BackupProgressInMegaBytes\": {},\n    \"CurrentBackupRateInMegaBytesPerSecond\": {},\n    \"EstimatedSecondsToCompletion\": {},\n    \"ElapsedTimeInSeconds\": {},\n    \"SourceRegion\": {},\n    \"Tags\": {},\n    \"RestorableNodeTypes\": {},\n    \"EnhancedVpcRouting\": {},\n    \"\
  MaintenanceTrackName\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"ManualSnapshotRemainingDays\": {},\n    \"SnapshotRetentionStartTime\": {}\n  },\n  \"description\": \"Describes a snapshot.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-schema.json\",\n  \"title\": \"Snapshot\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: Snapshot
---
