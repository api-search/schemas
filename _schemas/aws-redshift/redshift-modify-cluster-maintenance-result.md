---
description: ModifyClusterMaintenanceResult schema from Amazon Redshift
layout: schema
name: ModifyClusterMaintenanceResult
properties_list:
- description: Describes a cluster.
  name: Cluster
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-maintenance-result-schema.json
slug: redshift-modify-cluster-maintenance-result
source_filename: redshift-modify-cluster-maintenance-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cluster\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ClusterIdentifier\": {},\n        \"NodeType\": {},\n        \"ClusterStatus\": {},\n        \"ClusterAvailabilityStatus\": {},\n        \"ModifyStatus\": {},\n        \"MasterUsername\": {},\n        \"DBName\": {},\n        \"Endpoint\": {},\n        \"ClusterCreateTime\": {},\n        \"AutomatedSnapshotRetentionPeriod\": {},\n        \"ManualSnapshotRetentionPeriod\": {},\n        \"ClusterSecurityGroups\": {},\n        \"VpcSecurityGroups\": {},\n        \"ClusterParameterGroups\": {},\n        \"ClusterSubnetGroupName\": {},\n        \"VpcId\": {},\n        \"AvailabilityZone\": {},\n        \"PreferredMaintenanceWindow\": {},\n        \"PendingModifiedValues\": {},\n        \"ClusterVersion\": {},\n        \"AllowVersionUpgrade\": {},\n        \"NumberOfNodes\": {},\n        \"PubliclyAccessible\": {},\n        \"Encrypted\": {},\n    \
  \    \"RestoreStatus\": {},\n        \"DataTransferProgress\": {},\n        \"HsmStatus\": {},\n        \"ClusterSnapshotCopyStatus\": {},\n        \"ClusterPublicKey\": {},\n        \"ClusterNodes\": {},\n        \"ElasticIpStatus\": {},\n        \"ClusterRevisionNumber\": {},\n        \"Tags\": {},\n        \"KmsKeyId\": {},\n        \"EnhancedVpcRouting\": {},\n        \"IamRoles\": {},\n        \"PendingActions\": {},\n        \"MaintenanceTrackName\": {},\n        \"ElasticResizeNumberOfNodeOptions\": {},\n        \"DeferredMaintenanceWindows\": {},\n        \"SnapshotScheduleIdentifier\": {},\n        \"SnapshotScheduleState\": {},\n        \"ExpectedNextSnapshotScheduleTime\": {},\n        \"ExpectedNextSnapshotScheduleTimeStatus\": {},\n        \"NextMaintenanceWindowStartTime\": {},\n        \"ResizeInfo\": {},\n        \"AvailabilityZoneRelocationStatus\": {},\n        \"ClusterNamespaceArn\": {},\n        \"TotalStorageCapacityInMegaBytes\": {},\n        \"AquaConfiguration\"\
  : {},\n        \"DefaultIamRoleArn\": {},\n        \"ReservedNodeExchangeStatus\": {}\n      },\n      \"description\": \"Describes a cluster.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-maintenance-result-schema.json\",\n  \"title\": \"ModifyClusterMaintenanceResult\",\n  \"description\": \"ModifyClusterMaintenanceResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-maintenance-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterMaintenanceResult
---
