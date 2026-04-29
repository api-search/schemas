---
description: Describes a cluster.
layout: schema
name: Cluster
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: NodeType
  type: object
- description: ''
  name: ClusterStatus
  type: object
- description: ''
  name: ClusterAvailabilityStatus
  type: object
- description: ''
  name: ModifyStatus
  type: object
- description: ''
  name: MasterUsername
  type: object
- description: ''
  name: DBName
  type: object
- description: ''
  name: Endpoint
  type: object
- description: ''
  name: ClusterCreateTime
  type: object
- description: ''
  name: AutomatedSnapshotRetentionPeriod
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
- description: ''
  name: ClusterSecurityGroups
  type: object
- description: ''
  name: VpcSecurityGroups
  type: object
- description: ''
  name: ClusterParameterGroups
  type: object
- description: ''
  name: ClusterSubnetGroupName
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: PreferredMaintenanceWindow
  type: object
- description: ''
  name: PendingModifiedValues
  type: object
- description: ''
  name: ClusterVersion
  type: object
- description: ''
  name: AllowVersionUpgrade
  type: object
- description: ''
  name: NumberOfNodes
  type: object
- description: ''
  name: PubliclyAccessible
  type: object
- description: ''
  name: Encrypted
  type: object
- description: ''
  name: RestoreStatus
  type: object
- description: ''
  name: DataTransferProgress
  type: object
- description: ''
  name: HsmStatus
  type: object
- description: ''
  name: ClusterSnapshotCopyStatus
  type: object
- description: ''
  name: ClusterPublicKey
  type: object
- description: ''
  name: ClusterNodes
  type: object
- description: ''
  name: ElasticIpStatus
  type: object
- description: ''
  name: ClusterRevisionNumber
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: EnhancedVpcRouting
  type: object
- description: ''
  name: IamRoles
  type: object
- description: ''
  name: PendingActions
  type: object
- description: ''
  name: MaintenanceTrackName
  type: object
- description: ''
  name: ElasticResizeNumberOfNodeOptions
  type: object
- description: ''
  name: DeferredMaintenanceWindows
  type: object
- description: ''
  name: SnapshotScheduleIdentifier
  type: object
- description: ''
  name: SnapshotScheduleState
  type: object
- description: ''
  name: ExpectedNextSnapshotScheduleTime
  type: object
- description: ''
  name: ExpectedNextSnapshotScheduleTimeStatus
  type: object
- description: ''
  name: NextMaintenanceWindowStartTime
  type: object
- description: ''
  name: ResizeInfo
  type: object
- description: ''
  name: AvailabilityZoneRelocationStatus
  type: object
- description: ''
  name: ClusterNamespaceArn
  type: object
- description: ''
  name: TotalStorageCapacityInMegaBytes
  type: object
- description: ''
  name: AquaConfiguration
  type: object
- description: ''
  name: DefaultIamRoleArn
  type: object
- description: ''
  name: ReservedNodeExchangeStatus
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-schema.json
slug: redshift-cluster
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"NodeType\": {},\n    \"ClusterStatus\": {},\n    \"ClusterAvailabilityStatus\": {},\n    \"ModifyStatus\": {},\n    \"MasterUsername\": {},\n    \"DBName\": {},\n    \"Endpoint\": {},\n    \"ClusterCreateTime\": {},\n    \"AutomatedSnapshotRetentionPeriod\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"ClusterSecurityGroups\": {},\n    \"VpcSecurityGroups\": {},\n    \"ClusterParameterGroups\": {},\n    \"ClusterSubnetGroupName\": {},\n    \"VpcId\": {},\n    \"AvailabilityZone\": {},\n    \"PreferredMaintenanceWindow\": {},\n    \"PendingModifiedValues\": {},\n    \"ClusterVersion\": {},\n    \"AllowVersionUpgrade\": {},\n    \"NumberOfNodes\": {},\n    \"PubliclyAccessible\": {},\n    \"Encrypted\": {},\n    \"RestoreStatus\": {},\n    \"DataTransferProgress\": {},\n    \"HsmStatus\": {},\n    \"ClusterSnapshotCopyStatus\": {},\n    \"ClusterPublicKey\": {},\n    \"ClusterNodes\"\
  : {},\n    \"ElasticIpStatus\": {},\n    \"ClusterRevisionNumber\": {},\n    \"Tags\": {},\n    \"KmsKeyId\": {},\n    \"EnhancedVpcRouting\": {},\n    \"IamRoles\": {},\n    \"PendingActions\": {},\n    \"MaintenanceTrackName\": {},\n    \"ElasticResizeNumberOfNodeOptions\": {},\n    \"DeferredMaintenanceWindows\": {},\n    \"SnapshotScheduleIdentifier\": {},\n    \"SnapshotScheduleState\": {},\n    \"ExpectedNextSnapshotScheduleTime\": {},\n    \"ExpectedNextSnapshotScheduleTimeStatus\": {},\n    \"NextMaintenanceWindowStartTime\": {},\n    \"ResizeInfo\": {},\n    \"AvailabilityZoneRelocationStatus\": {},\n    \"ClusterNamespaceArn\": {},\n    \"TotalStorageCapacityInMegaBytes\": {},\n    \"AquaConfiguration\": {},\n    \"DefaultIamRoleArn\": {},\n    \"ReservedNodeExchangeStatus\": {}\n  },\n  \"description\": \"Describes a cluster.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-schema.json\"\
  ,\n  \"title\": \"Cluster\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: Cluster
---
