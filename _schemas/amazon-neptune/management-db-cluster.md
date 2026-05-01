---
description: Contains the details of an Amazon Neptune DB cluster.
layout: schema
name: DBCluster
properties_list:
- description: The user-supplied DB cluster identifier.
  name: DBClusterIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB cluster.
  name: DBClusterArn
  type: string
- description: Current state of the cluster.
  name: Status
  type: string
- description: The database engine (neptune).
  name: Engine
  type: string
- description: The version of the database engine.
  name: EngineVersion
  type: string
- description: The connection endpoint for the primary instance.
  name: Endpoint
  type: string
- description: The reader endpoint for read replicas.
  name: ReaderEndpoint
  type: string
- description: The port that the DB cluster listens on.
  name: Port
  type: integer
- description: The master username for the cluster.
  name: MasterUsername
  type: string
- description: The name of the DB cluster parameter group.
  name: DBClusterParameterGroup
  type: string
- description: The DB subnet group associated with the cluster.
  name: DBSubnetGroup
  type: string
- description: The allocated storage size in gigabytes.
  name: AllocatedStorage
  type: integer
- description: The time when the DB cluster was created.
  name: ClusterCreateTime
  type: string
- description: The daily time range for automated backups.
  name: PreferredBackupWindow
  type: string
- description: The weekly time range for system maintenance.
  name: PreferredMaintenanceWindow
  type: string
- description: Whether the cluster is Multi-AZ enabled.
  name: MultiAZ
  type: boolean
- description: Whether the cluster storage is encrypted.
  name: StorageEncrypted
  type: boolean
- description: The KMS key identifier for encrypted clusters.
  name: KmsKeyId
  type: string
- description: Whether deletion protection is enabled.
  name: DeletionProtection
  type: boolean
- description: Whether IAM database authentication is enabled.
  name: IAMDatabaseAuthenticationEnabled
  type: boolean
- description: The list of instances in the cluster.
  name: DBClusterMembers
  type: array
- description: IAM roles associated with the cluster.
  name: AssociatedRoles
  type: array
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-db-cluster-schema.json
slug: management-db-cluster
source_filename: management-db-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-schema.json\",\n  \"title\": \"DBCluster\",\n  \"description\": \"Contains the details of an Amazon Neptune DB cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied DB cluster identifier.\"\n    },\n    \"DBClusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB cluster.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the cluster.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine (neptune).\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the database engine.\"\
  \n    },\n    \"Endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The connection endpoint for the primary instance.\"\n    },\n    \"ReaderEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The reader endpoint for read replicas.\"\n    },\n    \"Port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port that the DB cluster listens on.\"\n    },\n    \"MasterUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The master username for the cluster.\"\n    },\n    \"DBClusterParameterGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the DB cluster parameter group.\"\n    },\n    \"DBSubnetGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The DB subnet group associated with the cluster.\"\n    },\n    \"AllocatedStorage\": {\n      \"type\": \"integer\",\n      \"description\": \"The allocated storage size in gigabytes.\"\n    },\n    \"ClusterCreateTime\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the DB cluster was created.\"\n    },\n    \"PreferredBackupWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The daily time range for automated backups.\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The weekly time range for system maintenance.\"\n    },\n    \"MultiAZ\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster is Multi-AZ enabled.\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster storage is encrypted.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The KMS key identifier for encrypted clusters.\"\n    },\n    \"DeletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether deletion protection is enabled.\"\n    },\n    \"IAMDatabaseAuthenticationEnabled\": {\n    \
  \  \"type\": \"boolean\",\n      \"description\": \"Whether IAM database authentication is enabled.\"\n    },\n    \"DBClusterMembers\": {\n      \"type\": \"array\",\n      \"description\": \"The list of instances in the cluster.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBClusterMember\"\n      }\n    },\n    \"AssociatedRoles\": {\n      \"type\": \"array\",\n      \"description\": \"IAM roles associated with the cluster.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBClusterRole\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DBCluster
---
