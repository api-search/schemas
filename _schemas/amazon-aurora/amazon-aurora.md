---
description: Schema defining the structure of an Amazon Aurora DB cluster resource, including cluster configuration, instances, endpoints, storage, backup, and security settings.
layout: schema
name: Amazon Aurora DB Cluster
properties_list:
- description: The user-supplied DB cluster identifier.
  name: DBClusterIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB cluster.
  name: DBClusterArn
  type: string
- description: The database engine for the DB cluster.
  name: Engine
  type: string
- description: The version of the database engine.
  name: EngineVersion
  type: string
- description: The current state of the DB cluster.
  name: Status
  type: string
- description: The connection endpoint for the primary instance of the DB cluster.
  name: Endpoint
  type: string
- description: The reader endpoint for the DB cluster.
  name: ReaderEndpoint
  type: string
- description: The port that the database engine is listening on.
  name: Port
  type: integer
- description: The master username for the DB cluster.
  name: MasterUsername
  type: string
- description: The name of the initial database created when the cluster was created.
  name: DatabaseName
  type: string
- description: The list of DB instances that make up the DB cluster.
  name: DBClusterMembers
  type: array
- description: The list of Availability Zones that instances in the DB cluster can be created in.
  name: AvailabilityZones
  type: array
- description: The number of days for which automatic DB snapshots are retained.
  name: BackupRetentionPeriod
  type: integer
- description: The daily time range during which automated backups are created.
  name: PreferredBackupWindow
  type: string
- description: The weekly time range during which system maintenance can occur.
  name: PreferredMaintenanceWindow
  type: string
- description: Whether the DB cluster is encrypted.
  name: StorageEncrypted
  type: boolean
- description: The AWS KMS key identifier for the encrypted DB cluster.
  name: KmsKeyId
  type: string
- description: Whether the DB cluster has deletion protection enabled.
  name: DeletionProtection
  type: boolean
- description: The list of VPC security groups that the DB cluster belongs to.
  name: VpcSecurityGroups
  type: array
- description: The name of the DB subnet group associated with the DB cluster.
  name: DBSubnetGroup
  type: string
- description: The time when the DB cluster was created.
  name: ClusterCreateTime
  type: string
- description: Tags associated with the DB cluster.
  name: Tags
  type: array
provider_name: Amazon Aurora
provider_slug: amazon-aurora
schema_file: json-schema/amazon-aurora-schema.json
slug: amazon-aurora
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-aurora/db-cluster\",\n  \"title\": \"Amazon Aurora DB Cluster\",\n  \"description\": \"Schema defining the structure of an Amazon Aurora DB cluster resource, including cluster configuration, instances, endpoints, storage, backup, and security settings.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DBClusterIdentifier\",\n    \"Engine\"\n  ],\n  \"properties\": {\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied DB cluster identifier.\",\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9-]*$\",\n      \"maxLength\": 63\n    },\n    \"DBClusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB cluster.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine for the DB cluster.\",\n      \"enum\": [\n\
  \        \"aurora-mysql\",\n        \"aurora-postgresql\"\n      ]\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the database engine.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the DB cluster.\"\n    },\n    \"Endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The connection endpoint for the primary instance of the DB cluster.\"\n    },\n    \"ReaderEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The reader endpoint for the DB cluster.\"\n    },\n    \"Port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port that the database engine is listening on.\"\n    },\n    \"MasterUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The master username for the DB cluster.\"\n    },\n    \"DatabaseName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the initial database created when\
  \ the cluster was created.\"\n    },\n    \"DBClusterMembers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DBClusterMember\"\n      },\n      \"description\": \"The list of DB instances that make up the DB cluster.\"\n    },\n    \"AvailabilityZones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The list of Availability Zones that instances in the DB cluster can be created in.\"\n    },\n    \"BackupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 35,\n      \"description\": \"The number of days for which automatic DB snapshots are retained.\"\n    },\n    \"PreferredBackupWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The daily time range during which automated backups are created.\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The weekly time range during which\
  \ system maintenance can occur.\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB cluster is encrypted.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS KMS key identifier for the encrypted DB cluster.\"\n    },\n    \"DeletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB cluster has deletion protection enabled.\"\n    },\n    \"VpcSecurityGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/VpcSecurityGroupMembership\"\n      },\n      \"description\": \"The list of VPC security groups that the DB cluster belongs to.\"\n    },\n    \"DBSubnetGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the DB subnet group associated with the DB cluster.\"\n    },\n    \"ClusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when\
  \ the DB cluster was created.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"description\": \"Tags associated with the DB cluster.\"\n    }\n  },\n  \"$defs\": {\n    \"DBClusterMember\": {\n      \"type\": \"object\",\n      \"description\": \"A member of a DB cluster.\",\n      \"properties\": {\n        \"DBInstanceIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"The instance identifier for the DB cluster member.\"\n        },\n        \"IsClusterWriter\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the cluster member is the primary instance.\"\n        },\n        \"DBClusterParameterGroupStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the DB cluster parameter group.\"\n        },\n        \"PromotionTier\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 15,\n  \
  \        \"description\": \"The failover priority order for the DB instance.\"\n        }\n      }\n    },\n    \"VpcSecurityGroupMembership\": {\n      \"type\": \"object\",\n      \"description\": \"A VPC security group associated with the DB cluster.\",\n      \"properties\": {\n        \"VpcSecurityGroupId\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the VPC security group.\"\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"description\": \"The membership status of the VPC security group.\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair for tagging AWS resources.\",\n      \"required\": [\n        \"Key\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag.\",\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n       \
  \   \"description\": \"The value of the tag.\",\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/json-schema/amazon-aurora-schema.json
tags:
- Amazon Aurora
- MySQL
- PostgreSQL
- Relational Database
- AWS
title: Amazon Aurora DB Cluster
---
