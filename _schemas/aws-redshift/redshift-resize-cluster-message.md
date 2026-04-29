---
description: Describes a resize cluster operation. For example, a scheduled action to run the <code>ResizeCluster</code> API operation.
layout: schema
name: ResizeClusterMessage
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
  name: Classic
  type: object
- description: ''
  name: ReservedNodeId
  type: object
- description: ''
  name: TargetReservedNodeOfferingId
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-resize-cluster-message-schema.json
slug: redshift-resize-cluster-message
source_filename: redshift-resize-cluster-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"ClusterType\": {},\n    \"NodeType\": {},\n    \"NumberOfNodes\": {},\n    \"Classic\": {},\n    \"ReservedNodeId\": {},\n    \"TargetReservedNodeOfferingId\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"Describes a resize cluster operation. For example, a scheduled action to run the <code>ResizeCluster</code> API operation. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-resize-cluster-message-schema.json\",\n  \"title\": \"ResizeClusterMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-resize-cluster-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ResizeClusterMessage
---
