---
description: Represents an Amazon Neptune DB instance, which is a compute node within a Neptune DB cluster that processes graph queries and manages the connection to the shared cluster storage.
layout: schema
name: Amazon Neptune DB Instance
properties_list:
- description: The user-supplied unique identifier for the DB instance.
  name: DBInstanceIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB instance.
  name: DBInstanceArn
  type: string
- description: The compute and memory capacity of the DB instance (e.g., db.r5.large, db.r6g.xlarge, db.serverless).
  name: DBInstanceClass
  type: string
- description: The name of the database engine.
  name: Engine
  type: string
- description: The version of the Neptune database engine.
  name: EngineVersion
  type: string
- description: The current state of the DB instance.
  name: DBInstanceStatus
  type: string
- description: The connection endpoint for the DB instance.
  name: Endpoint
  type: object
- description: The identifier of the DB cluster that this instance belongs to.
  name: DBClusterIdentifier
  type: string
- description: The name of the Availability Zone where the DB instance is located.
  name: AvailabilityZone
  type: string
- description: The DB subnet group associated with the instance.
  name: DBSubnetGroup
  type: object
- description: The weekly time range during which system maintenance can occur (UTC).
  name: PreferredMaintenanceWindow
  type: string
- description: Whether minor engine version upgrades are applied automatically.
  name: AutoMinorVersionUpgrade
  type: boolean
- description: Whether the DB instance is publicly accessible.
  name: PubliclyAccessible
  type: boolean
- description: The order in which a read replica is promoted to the primary instance during a failover.
  name: PromotionTier
  type: integer
- description: Whether the DB instance storage is encrypted.
  name: StorageEncrypted
  type: boolean
- description: The AWS KMS key identifier for the encrypted instance.
  name: KmsKeyId
  type: string
- description: The AWS Region-unique, immutable identifier for the DB instance.
  name: DbiResourceId
  type: string
- description: The identifier of the CA certificate for this DB instance.
  name: CACertificateIdentifier
  type: string
- description: Whether tags are copied to snapshots of the DB instance.
  name: CopyTagsToSnapshot
  type: boolean
- description: The date and time when the DB instance was created.
  name: InstanceCreateTime
  type: string
- description: Changes to the DB instance that are pending application.
  name: PendingModifiedValues
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/amazon-neptune-db-instance-schema.json
slug: amazon-neptune-db-instance
source_filename: amazon-neptune-db-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/amazon-neptune/json-schema/amazon-neptune-db-instance-schema.json\",\n  \"title\": \"Amazon Neptune DB Instance\",\n  \"description\": \"Represents an Amazon Neptune DB instance, which is a compute node within a Neptune DB cluster that processes graph queries and manages the connection to the shared cluster storage.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DBInstanceIdentifier\",\n    \"DBInstanceClass\",\n    \"Engine\"\n  ],\n  \"properties\": {\n    \"DBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied unique identifier for the DB instance.\",\n      \"minLength\": 1,\n      \"maxLength\": 63\n    },\n    \"DBInstanceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB instance.\"\n    },\n    \"DBInstanceClass\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"The compute and memory capacity of the DB instance (e.g., db.r5.large, db.r6g.xlarge, db.serverless).\",\n      \"examples\": [\n        \"db.r5.large\",\n        \"db.r5.xlarge\",\n        \"db.r6g.large\",\n        \"db.t3.medium\",\n        \"db.serverless\"\n      ]\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database engine.\",\n      \"const\": \"neptune\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the Neptune database engine.\"\n    },\n    \"DBInstanceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the DB instance.\",\n      \"enum\": [\n        \"available\",\n        \"backing-up\",\n        \"creating\",\n        \"deleting\",\n        \"failed\",\n        \"inaccessible-encryption-credentials\",\n        \"incompatible-network\",\n        \"incompatible-option-group\",\n        \"incompatible-parameters\"\
  ,\n        \"incompatible-restore\",\n        \"maintenance\",\n        \"modifying\",\n        \"rebooting\",\n        \"renaming\",\n        \"starting\",\n        \"stopped\",\n        \"stopping\",\n        \"storage-optimization\",\n        \"upgrading\"\n      ]\n    },\n    \"Endpoint\": {\n      \"type\": \"object\",\n      \"description\": \"The connection endpoint for the DB instance.\",\n      \"properties\": {\n        \"Address\": {\n          \"type\": \"string\",\n          \"description\": \"The DNS address of the DB instance.\"\n        },\n        \"Port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port that the DB instance listens on.\",\n          \"default\": 8182\n        },\n        \"HostedZoneId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the hosted zone for the endpoint.\"\n        }\n      }\n    },\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier\
  \ of the DB cluster that this instance belongs to.\"\n    },\n    \"AvailabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Availability Zone where the DB instance is located.\"\n    },\n    \"DBSubnetGroup\": {\n      \"type\": \"object\",\n      \"description\": \"The DB subnet group associated with the instance.\",\n      \"properties\": {\n        \"DBSubnetGroupName\": {\n          \"type\": \"string\"\n        },\n        \"DBSubnetGroupDescription\": {\n          \"type\": \"string\"\n        },\n        \"VpcId\": {\n          \"type\": \"string\"\n        },\n        \"SubnetGroupStatus\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The weekly time range during which system maintenance can occur (UTC).\"\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether minor engine version\
  \ upgrades are applied automatically.\"\n    },\n    \"PubliclyAccessible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB instance is publicly accessible.\",\n      \"default\": false\n    },\n    \"PromotionTier\": {\n      \"type\": \"integer\",\n      \"description\": \"The order in which a read replica is promoted to the primary instance during a failover.\",\n      \"minimum\": 0,\n      \"maximum\": 15,\n      \"default\": 1\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB instance storage is encrypted.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS KMS key identifier for the encrypted instance.\"\n    },\n    \"DbiResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS Region-unique, immutable identifier for the DB instance.\"\n    },\n    \"CACertificateIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The identifier of the CA certificate for this DB instance.\"\n    },\n    \"CopyTagsToSnapshot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether tags are copied to snapshots of the DB instance.\"\n    },\n    \"InstanceCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the DB instance was created.\"\n    },\n    \"PendingModifiedValues\": {\n      \"type\": \"object\",\n      \"description\": \"Changes to the DB instance that are pending application.\",\n      \"properties\": {\n        \"DBInstanceClass\": {\n          \"type\": \"string\"\n        },\n        \"EngineVersion\": {\n          \"type\": \"string\"\n        },\n        \"PendingCloudwatchLogsExports\": {\n          \"type\": \"object\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/amazon-neptune-db-instance-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: Amazon Neptune DB Instance
---
