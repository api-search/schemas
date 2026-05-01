---
description: Represents an Amazon Neptune DB cluster, which is a managed graph database cluster with one writer instance and up to 15 read replica instances sharing a distributed storage volume.
layout: schema
name: Amazon Neptune DB Cluster
properties_list:
- description: The user-supplied unique identifier for the DB cluster. Must contain 1-63 alphanumeric characters or hyphens, start with a letter, and not end with a hyphen.
  name: DBClusterIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB cluster.
  name: DBClusterArn
  type: string
- description: The current state of the DB cluster.
  name: Status
  type: string
- description: The name of the database engine (always 'neptune').
  name: Engine
  type: string
- description: The version of the Neptune database engine.
  name: EngineVersion
  type: string
- description: The DNS address of the primary instance of the DB cluster. This is the read/write cluster endpoint.
  name: Endpoint
  type: string
- description: The reader endpoint for the DB cluster. Used to distribute read-only connections across read replicas.
  name: ReaderEndpoint
  type: string
- description: The port that the DB cluster listens on.
  name: Port
  type: integer
- description: The name of the DB cluster parameter group associated with the cluster.
  name: DBClusterParameterGroup
  type: string
- description: The name of the DB subnet group associated with the cluster.
  name: DBSubnetGroup
  type: string
- description: The allocated storage size in gibibytes (GiB).
  name: AllocatedStorage
  type: integer
- description: The time when the DB cluster was created, in UTC.
  name: ClusterCreateTime
  type: string
- description: The daily time range during which automated backups are created (UTC), in the format hh24:mi-hh24:mi.
  name: PreferredBackupWindow
  type: string
- description: The weekly time range during which system maintenance can occur (UTC), in the format ddd:hh24:mi-ddd:hh24:mi.
  name: PreferredMaintenanceWindow
  type: string
- description: The number of days for which automated backups are retained.
  name: BackupRetentionPeriod
  type: integer
- description: Whether the DB cluster has instances in multiple Availability Zones.
  name: MultiAZ
  type: boolean
- description: Whether the DB cluster storage is encrypted at rest.
  name: StorageEncrypted
  type: boolean
- description: The AWS KMS key identifier used for encrypting the cluster storage.
  name: KmsKeyId
  type: string
- description: Whether deletion protection is enabled. When enabled, the cluster cannot be deleted.
  name: DeletionProtection
  type: boolean
- description: Whether AWS Identity and Access Management (IAM) database authentication is enabled.
  name: IAMDatabaseAuthenticationEnabled
  type: boolean
- description: The list of DB instances that are members of this cluster.
  name: DBClusterMembers
  type: array
- description: The VPC security groups associated with the cluster.
  name: VpcSecurityGroups
  type: array
- description: IAM roles that are associated with the DB cluster for accessing other AWS services.
  name: AssociatedRoles
  type: array
- description: The Availability Zones in which instances in the cluster can be created.
  name: AvailabilityZones
  type: array
- description: Whether tags are copied to snapshots of the DB cluster.
  name: CopyTagsToSnapshot
  type: boolean
- description: Whether the cluster can be cloned across accounts.
  name: CrossAccountClone
  type: boolean
- description: The scaling configuration for Neptune Serverless.
  name: ServerlessV2ScalingConfiguration
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/amazon-neptune-db-cluster-schema.json
slug: amazon-neptune-db-cluster
source_filename: amazon-neptune-db-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/amazon-neptune/json-schema/amazon-neptune-db-cluster-schema.json\",\n  \"title\": \"Amazon Neptune DB Cluster\",\n  \"description\": \"Represents an Amazon Neptune DB cluster, which is a managed graph database cluster with one writer instance and up to 15 read replica instances sharing a distributed storage volume.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DBClusterIdentifier\",\n    \"Engine\"\n  ],\n  \"properties\": {\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied unique identifier for the DB cluster. Must contain 1-63 alphanumeric characters or hyphens, start with a letter, and not end with a hyphen.\",\n      \"minLength\": 1,\n      \"maxLength\": 63,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9-]*[a-zA-Z0-9]$\"\n    },\n    \"DBClusterArn\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The Amazon Resource Name (ARN) for the DB cluster.\",\n      \"pattern\": \"^arn:aws[a-z-]*:rds:[a-z0-9-]+:[0-9]+:cluster:\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the DB cluster.\",\n      \"enum\": [\n        \"available\",\n        \"backing-up\",\n        \"creating\",\n        \"deleting\",\n        \"failing-over\",\n        \"inaccessible-encryption-credentials\",\n        \"maintenance\",\n        \"migrating\",\n        \"modifying\",\n        \"promoting\",\n        \"renaming\",\n        \"resetting-master-credentials\",\n        \"starting\",\n        \"stopped\",\n        \"stopping\",\n        \"upgrading\"\n      ]\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database engine (always 'neptune').\",\n      \"const\": \"neptune\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the Neptune database engine.\"\
  ,\n      \"examples\": [\n        \"1.2.1.0\",\n        \"1.3.0.0\",\n        \"1.3.1.0\"\n      ]\n    },\n    \"Endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS address of the primary instance of the DB cluster. This is the read/write cluster endpoint.\"\n    },\n    \"ReaderEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The reader endpoint for the DB cluster. Used to distribute read-only connections across read replicas.\"\n    },\n    \"Port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port that the DB cluster listens on.\",\n      \"default\": 8182\n    },\n    \"DBClusterParameterGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the DB cluster parameter group associated with the cluster.\"\n    },\n    \"DBSubnetGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the DB subnet group associated with the cluster.\"\n    },\n    \"AllocatedStorage\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"The allocated storage size in gibibytes (GiB).\"\n    },\n    \"ClusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the DB cluster was created, in UTC.\"\n    },\n    \"PreferredBackupWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The daily time range during which automated backups are created (UTC), in the format hh24:mi-hh24:mi.\",\n      \"pattern\": \"^[0-2][0-9]:[0-5][0-9]-[0-2][0-9]:[0-5][0-9]$\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The weekly time range during which system maintenance can occur (UTC), in the format ddd:hh24:mi-ddd:hh24:mi.\"\n    },\n    \"BackupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which automated backups are retained.\",\n      \"minimum\": 1,\n      \"maximum\": 35\n    },\n    \"MultiAZ\": {\n \
  \     \"type\": \"boolean\",\n      \"description\": \"Whether the DB cluster has instances in multiple Availability Zones.\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB cluster storage is encrypted at rest.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS KMS key identifier used for encrypting the cluster storage.\"\n    },\n    \"DeletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether deletion protection is enabled. When enabled, the cluster cannot be deleted.\",\n      \"default\": false\n    },\n    \"IAMDatabaseAuthenticationEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether AWS Identity and Access Management (IAM) database authentication is enabled.\"\n    },\n    \"DBClusterMembers\": {\n      \"type\": \"array\",\n      \"description\": \"The list of DB instances that are members of this cluster.\",\n      \"items\"\
  : {\n        \"$ref\": \"#/$defs/DBClusterMember\"\n      }\n    },\n    \"VpcSecurityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The VPC security groups associated with the cluster.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"VpcSecurityGroupId\": {\n            \"type\": \"string\"\n          },\n          \"Status\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"AssociatedRoles\": {\n      \"type\": \"array\",\n      \"description\": \"IAM roles that are associated with the DB cluster for accessing other AWS services.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DBClusterRole\"\n      }\n    },\n    \"AvailabilityZones\": {\n      \"type\": \"array\",\n      \"description\": \"The Availability Zones in which instances in the cluster can be created.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CopyTagsToSnapshot\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether tags are copied to snapshots of the DB cluster.\"\n    },\n    \"CrossAccountClone\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster can be cloned across accounts.\"\n    },\n    \"ServerlessV2ScalingConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The scaling configuration for Neptune Serverless.\",\n      \"properties\": {\n        \"MinCapacity\": {\n          \"type\": \"number\",\n          \"description\": \"The minimum number of Neptune capacity units (NCUs).\"\n        },\n        \"MaxCapacity\": {\n          \"type\": \"number\",\n          \"description\": \"The maximum number of Neptune capacity units (NCUs).\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"DBClusterMember\": {\n      \"type\": \"object\",\n      \"description\": \"A DB instance that is a member of a Neptune DB cluster.\",\n      \"properties\": {\n        \"DBInstanceIdentifier\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The instance identifier for this member.\"\n        },\n        \"IsClusterWriter\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this instance is the primary (writer) instance of the cluster.\"\n        },\n        \"DBClusterParameterGroupStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the DB cluster parameter group for this member.\"\n        },\n        \"PromotionTier\": {\n          \"type\": \"integer\",\n          \"description\": \"The failover priority order. Lower values have higher priority.\",\n          \"minimum\": 0,\n          \"maximum\": 15\n        }\n      }\n    },\n    \"DBClusterRole\": {\n      \"type\": \"object\",\n      \"description\": \"An IAM role associated with a Neptune DB cluster.\",\n      \"properties\": {\n        \"RoleArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the IAM role.\"\n        },\n     \
  \   \"Status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the association between the IAM role and the cluster.\",\n          \"enum\": [\n            \"active\",\n            \"pending\",\n            \"error\"\n          ]\n        },\n        \"FeatureName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the feature associated with the role.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/amazon-neptune-db-cluster-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: Amazon Neptune DB Cluster
---
