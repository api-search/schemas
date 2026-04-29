---
description: Schema representing an Amazon DocumentDB database cluster, which is a managed MongoDB-compatible document database cluster consisting of one or more instances connected to a shared storage volume.
layout: schema
name: Amazon DocumentDB DBCluster
properties_list:
- description: The user-supplied DB cluster identifier. This identifier is the unique key that identifies a DB cluster.
  name: DBClusterIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB cluster.
  name: DBClusterArn
  type: string
- description: Specifies the current state of this DB cluster.
  name: Status
  type: string
- description: The name of the database engine to be used for this DB cluster.
  name: Engine
  type: string
- description: Indicates the database engine version.
  name: EngineVersion
  type: string
- description: The connection endpoint for the primary instance of the DB cluster.
  name: Endpoint
  type: string
- description: The reader endpoint for the DB cluster. The reader endpoint load-balances connections across the read replicas.
  name: ReaderEndpoint
  type: string
- description: Specifies the port that the database engine is listening on.
  name: Port
  type: integer
- description: Contains the master username for the DB cluster.
  name: MasterUsername
  type: string
- description: Specifies information on the subnet group associated with the DB cluster.
  name: DBSubnetGroup
  type: string
- description: Specifies whether the DB cluster is encrypted.
  name: StorageEncrypted
  type: boolean
- description: If StorageEncrypted is true, the AWS KMS key identifier for the encrypted DB cluster.
  name: KmsKeyId
  type: string
- description: Specifies the number of days for which automatic DB snapshots are retained.
  name: BackupRetentionPeriod
  type: integer
- description: Specifies the daily time range during which automated backups are created.
  name: PreferredBackupWindow
  type: string
- description: Specifies the weekly time range during which system maintenance can occur.
  name: PreferredMaintenanceWindow
  type: string
- description: Specifies the time when the DB cluster was created, in Universal Coordinated Time (UTC).
  name: ClusterCreateTime
  type: string
- description: Provides the list of instances that make up the DB cluster.
  name: DBClusterMembers
  type: array
- description: Provides a list of VPC security groups that the DB cluster belongs to.
  name: VpcSecurityGroups
  type: array
- description: Specifies whether this cluster can be deleted. If DeletionProtection is enabled, the cluster cannot be deleted unless it is modified and DeletionProtection is disabled.
  name: DeletionProtection
  type: boolean
- description: A list of log types that this DB cluster is configured to export to Amazon CloudWatch Logs.
  name: EnabledCloudwatchLogsExports
  type: array
provider_name: Amazon DocumentDB
provider_slug: amazon-documentdb
schema_file: json-schema/amazon-documentdb-dbcluster-schema.json
slug: amazon-documentdb-dbcluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apis.io/schemas/amazon-documentdb-dbcluster.json\",\n  \"title\": \"Amazon DocumentDB DBCluster\",\n  \"description\": \"Schema representing an Amazon DocumentDB database cluster, which is a managed MongoDB-compatible document database cluster consisting of one or more instances connected to a shared storage volume.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DBClusterIdentifier\",\n    \"Engine\"\n  ],\n  \"properties\": {\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied DB cluster identifier. This identifier is the unique key that identifies a DB cluster.\",\n      \"minLength\": 1,\n      \"maxLength\": 63,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9-]*$\"\n    },\n    \"DBClusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB cluster.\",\n      \"pattern\":\
  \ \"^arn:aws[a-zA-Z-]*:rds:[a-z0-9-]+:[0-9]{12}:cluster:.+$\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the current state of this DB cluster.\",\n      \"enum\": [\n        \"available\",\n        \"backing-up\",\n        \"creating\",\n        \"deleting\",\n        \"failing-over\",\n        \"maintenance\",\n        \"migrating\",\n        \"modifying\",\n        \"renaming\",\n        \"resetting-master-credentials\",\n        \"upgrading\"\n      ]\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database engine to be used for this DB cluster.\",\n      \"const\": \"docdb\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the database engine version.\"\n    },\n    \"Endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The connection endpoint for the primary instance of the DB cluster.\",\n      \"format\": \"hostname\"\
  \n    },\n    \"ReaderEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The reader endpoint for the DB cluster. The reader endpoint load-balances connections across the read replicas.\",\n      \"format\": \"hostname\"\n    },\n    \"Port\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the port that the database engine is listening on.\",\n      \"default\": 27017\n    },\n    \"MasterUsername\": {\n      \"type\": \"string\",\n      \"description\": \"Contains the master username for the DB cluster.\"\n    },\n    \"DBSubnetGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies information on the subnet group associated with the DB cluster.\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the DB cluster is encrypted.\",\n      \"default\": false\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"If StorageEncrypted is true, the\
  \ AWS KMS key identifier for the encrypted DB cluster.\"\n    },\n    \"BackupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the number of days for which automatic DB snapshots are retained.\",\n      \"minimum\": 1,\n      \"maximum\": 35,\n      \"default\": 1\n    },\n    \"PreferredBackupWindow\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the daily time range during which automated backups are created.\",\n      \"pattern\": \"^([01]\\\\d|2[0-3]):[0-5]\\\\d-([01]\\\\d|2[0-3]):[0-5]\\\\d$\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the weekly time range during which system maintenance can occur.\"\n    },\n    \"ClusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Specifies the time when the DB cluster was created, in Universal Coordinated Time (UTC).\"\n    },\n    \"DBClusterMembers\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"Provides the list of instances that make up the DB cluster.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"DBInstanceIdentifier\": {\n            \"type\": \"string\",\n            \"description\": \"Specifies the instance identifier for this member of the DB cluster.\"\n          },\n          \"IsClusterWriter\": {\n            \"type\": \"boolean\",\n            \"description\": \"A value that is true if the cluster member is the primary instance for the DB cluster.\"\n          },\n          \"DBClusterParameterGroupStatus\": {\n            \"type\": \"string\",\n            \"description\": \"Specifies the status of the DB cluster parameter group for this member.\"\n          },\n          \"PromotionTier\": {\n            \"type\": \"integer\",\n            \"description\": \"A value that specifies the order in which a read replica is promoted to the primary instance.\",\n       \
  \     \"minimum\": 0,\n            \"maximum\": 15\n          }\n        }\n      }\n    },\n    \"VpcSecurityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Provides a list of VPC security groups that the DB cluster belongs to.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"VpcSecurityGroupId\": {\n            \"type\": \"string\"\n          },\n          \"Status\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"DeletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether this cluster can be deleted. If DeletionProtection is enabled, the cluster cannot be deleted unless it is modified and DeletionProtection is disabled.\",\n      \"default\": false\n    },\n    \"EnabledCloudwatchLogsExports\": {\n      \"type\": \"array\",\n      \"description\": \"A list of log types that this DB cluster is configured to export to Amazon CloudWatch Logs.\",\n  \
  \    \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"audit\",\n          \"profiler\"\n        ]\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/json-schema/amazon-documentdb-dbcluster-schema.json
tags:
- Amazon Web Services
- AWS
- Database
- Document Database
- DocumentDB
- Managed Database
- MongoDB
- NoSQL
title: Amazon DocumentDB DBCluster
---
