---
description: <p/>
layout: schema
name: ModifyClusterMessage
properties_list:
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
  name: NumberOfNodes
  type: object
- description: ''
  name: ClusterSecurityGroups
  type: object
- description: ''
  name: VpcSecurityGroupIds
  type: object
- description: ''
  name: MasterUserPassword
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
  name: PreferredMaintenanceWindow
  type: object
- description: ''
  name: ClusterVersion
  type: object
- description: ''
  name: AllowVersionUpgrade
  type: object
- description: ''
  name: HsmClientCertificateIdentifier
  type: object
- description: ''
  name: HsmConfigurationIdentifier
  type: object
- description: ''
  name: NewClusterIdentifier
  type: object
- description: ''
  name: PubliclyAccessible
  type: object
- description: ''
  name: ElasticIp
  type: object
- description: ''
  name: EnhancedVpcRouting
  type: object
- description: ''
  name: MaintenanceTrackName
  type: object
- description: ''
  name: Encrypted
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: AvailabilityZoneRelocation
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: Port
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-message-schema.json
slug: redshift-modify-cluster-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"ClusterType\": {},\n    \"NodeType\": {},\n    \"NumberOfNodes\": {},\n    \"ClusterSecurityGroups\": {},\n    \"VpcSecurityGroupIds\": {},\n    \"MasterUserPassword\": {},\n    \"ClusterParameterGroupName\": {},\n    \"AutomatedSnapshotRetentionPeriod\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"PreferredMaintenanceWindow\": {},\n    \"ClusterVersion\": {},\n    \"AllowVersionUpgrade\": {},\n    \"HsmClientCertificateIdentifier\": {},\n    \"HsmConfigurationIdentifier\": {},\n    \"NewClusterIdentifier\": {},\n    \"PubliclyAccessible\": {},\n    \"ElasticIp\": {},\n    \"EnhancedVpcRouting\": {},\n    \"MaintenanceTrackName\": {},\n    \"Encrypted\": {},\n    \"KmsKeyId\": {},\n    \"AvailabilityZoneRelocation\": {},\n    \"AvailabilityZone\": {},\n    \"Port\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-message-schema.json\",\n  \"title\": \"ModifyClusterMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterMessage
---
