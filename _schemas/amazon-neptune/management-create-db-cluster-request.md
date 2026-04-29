---
description: CreateDBClusterRequest schema from Neptune
layout: schema
name: CreateDBClusterRequest
properties_list:
- description: The DB cluster identifier.
  name: DBClusterIdentifier
  type: string
- description: The database engine to use (neptune).
  name: Engine
  type: string
- description: The version of the Neptune engine.
  name: EngineVersion
  type: string
- description: The port number on which the cluster accepts connections.
  name: Port
  type: integer
- description: The name of a DB subnet group.
  name: DBSubnetGroupName
  type: string
- description: A list of VPC security group IDs.
  name: VpcSecurityGroupIds
  type: array
- description: Whether the cluster is encrypted.
  name: StorageEncrypted
  type: boolean
- description: The KMS key identifier for an encrypted cluster.
  name: KmsKeyId
  type: string
- description: The daily time range for automated backups (UTC).
  name: PreferredBackupWindow
  type: string
- description: The weekly time range for maintenance (UTC).
  name: PreferredMaintenanceWindow
  type: string
- description: The number of days for which automated backups are retained (1-35).
  name: BackupRetentionPeriod
  type: integer
- description: Whether to enable deletion protection.
  name: DeletionProtection
  type: boolean
- description: Whether to enable IAM database authentication.
  name: IAMDatabaseAuthenticationEnabled
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-create-db-cluster-request-schema.json
slug: management-create-db-cluster-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-create-db-cluster-request-schema.json\",\n  \"title\": \"CreateDBClusterRequest\",\n  \"description\": \"CreateDBClusterRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The DB cluster identifier.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine to use (neptune).\",\n      \"default\": \"neptune\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the Neptune engine.\"\n    },\n    \"Port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number on which the cluster accepts connections.\",\n      \"default\": 8182\n    },\n    \"DBSubnetGroupName\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"The name of a DB subnet group.\"\n    },\n    \"VpcSecurityGroupIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of VPC security group IDs.\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster is encrypted.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The KMS key identifier for an encrypted cluster.\"\n    },\n    \"PreferredBackupWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The daily time range for automated backups (UTC).\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The weekly time range for maintenance (UTC).\"\n    },\n    \"BackupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which automated backups are retained (1-35).\"\
  \n    },\n    \"DeletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable deletion protection.\"\n    },\n    \"IAMDatabaseAuthenticationEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable IAM database authentication.\"\n    }\n  },\n  \"required\": [\n    \"DBClusterIdentifier\",\n    \"Engine\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-create-db-cluster-request-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateDBClusterRequest
---
