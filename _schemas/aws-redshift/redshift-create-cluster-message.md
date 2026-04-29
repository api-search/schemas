---
description: <p/>
layout: schema
name: CreateClusterMessage
properties_list:
- description: ''
  name: DBName
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: ClusterType
  type: object
- description: ''
  name: NodeType
  type: object
- description: ''
  name: MasterUsername
  type: object
- description: ''
  name: MasterUserPassword
  type: object
- description: ''
  name: ClusterSecurityGroups
  type: object
- description: ''
  name: VpcSecurityGroupIds
  type: object
- description: ''
  name: ClusterSubnetGroupName
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: PreferredMaintenanceWindow
  type: object
- description: ''
  name: ClusterParameterGroupName
  type: object
- description: ''
  name: AutomatedSnapshotRetentionPeriod
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
- description: ''
  name: Port
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
  name: HsmClientCertificateIdentifier
  type: object
- description: ''
  name: HsmConfigurationIdentifier
  type: object
- description: ''
  name: ElasticIp
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
  name: AdditionalInfo
  type: object
- description: ''
  name: IamRoles
  type: object
- description: ''
  name: MaintenanceTrackName
  type: object
- description: ''
  name: SnapshotScheduleIdentifier
  type: object
- description: ''
  name: AvailabilityZoneRelocation
  type: object
- description: ''
  name: AquaConfigurationStatus
  type: object
- description: ''
  name: DefaultIamRoleArn
  type: object
- description: ''
  name: LoadSampleData
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-cluster-message-schema.json
slug: redshift-create-cluster-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBName\": {},\n    \"ClusterIdentifier\": {},\n    \"ClusterType\": {},\n    \"NodeType\": {},\n    \"MasterUsername\": {},\n    \"MasterUserPassword\": {},\n    \"ClusterSecurityGroups\": {},\n    \"VpcSecurityGroupIds\": {},\n    \"ClusterSubnetGroupName\": {},\n    \"AvailabilityZone\": {},\n    \"PreferredMaintenanceWindow\": {},\n    \"ClusterParameterGroupName\": {},\n    \"AutomatedSnapshotRetentionPeriod\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"Port\": {},\n    \"ClusterVersion\": {},\n    \"AllowVersionUpgrade\": {},\n    \"NumberOfNodes\": {},\n    \"PubliclyAccessible\": {},\n    \"Encrypted\": {},\n    \"HsmClientCertificateIdentifier\": {},\n    \"HsmConfigurationIdentifier\": {},\n    \"ElasticIp\": {},\n    \"Tags\": {},\n    \"KmsKeyId\": {},\n    \"EnhancedVpcRouting\": {},\n    \"AdditionalInfo\": {},\n    \"IamRoles\": {},\n    \"MaintenanceTrackName\": {},\n    \"SnapshotScheduleIdentifier\"\
  : {},\n    \"AvailabilityZoneRelocation\": {},\n    \"AquaConfigurationStatus\": {},\n    \"DefaultIamRoleArn\": {},\n    \"LoadSampleData\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\",\n    \"NodeType\",\n    \"MasterUsername\",\n    \"MasterUserPassword\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-message-schema.json\",\n  \"title\": \"CreateClusterMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateClusterMessage
---
