---
description: Describes cluster attributes that are in a pending state. A change to one or more the attributes was requested and is in progress or will be applied.
layout: schema
name: PendingModifiedValues
properties_list:
- description: ''
  name: MasterUserPassword
  type: object
- description: ''
  name: NodeType
  type: object
- description: ''
  name: NumberOfNodes
  type: object
- description: ''
  name: ClusterType
  type: object
- description: ''
  name: ClusterVersion
  type: object
- description: ''
  name: AutomatedSnapshotRetentionPeriod
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: PubliclyAccessible
  type: object
- description: ''
  name: EnhancedVpcRouting
  type: object
- description: ''
  name: MaintenanceTrackName
  type: object
- description: ''
  name: EncryptionType
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-pending-modified-values-schema.json
slug: redshift-pending-modified-values
source_filename: redshift-pending-modified-values-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MasterUserPassword\": {},\n    \"NodeType\": {},\n    \"NumberOfNodes\": {},\n    \"ClusterType\": {},\n    \"ClusterVersion\": {},\n    \"AutomatedSnapshotRetentionPeriod\": {},\n    \"ClusterIdentifier\": {},\n    \"PubliclyAccessible\": {},\n    \"EnhancedVpcRouting\": {},\n    \"MaintenanceTrackName\": {},\n    \"EncryptionType\": {}\n  },\n  \"description\": \"Describes cluster attributes that are in a pending state. A change to one or more the attributes was requested and is in progress or will be applied.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-pending-modified-values-schema.json\",\n  \"title\": \"PendingModifiedValues\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-pending-modified-values-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: PendingModifiedValues
---
