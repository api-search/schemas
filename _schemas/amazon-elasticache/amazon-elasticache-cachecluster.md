---
description: Schema representing an Amazon ElastiCache cache cluster, which is a collection of cache nodes running Redis or Memcached cache engine software.
layout: schema
name: Amazon ElastiCache CacheCluster
properties_list:
- description: The user-supplied identifier of the cluster. This identifier is a unique key that identifies a cluster.
  name: CacheClusterId
  type: string
- description: The ARN (Amazon Resource Name) of the cache cluster.
  name: ARN
  type: string
- description: The current state of this cluster.
  name: CacheClusterStatus
  type: string
- description: The name of the cache engine used in this cluster.
  name: Engine
  type: string
- description: The version of the cache engine that is used in this cluster.
  name: EngineVersion
  type: string
- description: The name of the compute and memory capacity node type for the cluster.
  name: CacheNodeType
  type: string
- description: The number of cache nodes in the cluster.
  name: NumCacheNodes
  type: integer
- description: The name of the Availability Zone in which the cluster is located or "Multiple" if the cache nodes are located in different Availability Zones.
  name: PreferredAvailabilityZone
  type: string
- description: The date and time when the cluster was created.
  name: CacheClusterCreateTime
  type: string
- description: Specifies the weekly time range during which maintenance on the cluster is performed.
  name: PreferredMaintenanceWindow
  type: string
- description: The name of the cache subnet group associated with the cluster.
  name: CacheSubnetGroupName
  type: string
- description: Status of the cache parameter group.
  name: CacheParameterGroup
  type: object
- description: A list of cache nodes that are members of the cluster.
  name: CacheNodes
  type: array
- description: Represents a Memcached cluster endpoint which can be used by an application to connect to any node in the cluster.
  name: ConfigurationEndpoint
  type: object
- description: A list of VPC Security Groups associated with the cluster.
  name: SecurityGroups
  type: array
- description: The replication group to which this cluster belongs.
  name: ReplicationGroupId
  type:
  - string
  - 'null'
- description: The number of days for which ElastiCache retains automatic cluster snapshots.
  name: SnapshotRetentionLimit
  type: integer
- description: The daily time range (in UTC) during which ElastiCache begins taking a daily snapshot of your cluster.
  name: SnapshotWindow
  type: string
- description: If true, then minor version patches are applied automatically.
  name: AutoMinorVersionUpgrade
  type: boolean
- description: The port number on which each of the cache nodes accepts connections.
  name: Port
  type: integer
- description: Describes a notification topic and its status.
  name: NotificationConfiguration
  type: object
- description: A flag that enables in-transit encryption when set to true.
  name: TransitEncryptionEnabled
  type: boolean
- description: A flag that enables encryption at rest when set to true.
  name: AtRestEncryptionEnabled
  type: boolean
provider_name: Amazon ElastiCache
provider_slug: amazon-elasticache
schema_file: json-schema/amazon-elasticache-cachecluster-schema.json
slug: amazon-elasticache-cachecluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apis.io/schemas/amazon-elasticache-cachecluster.json\",\n  \"title\": \"Amazon ElastiCache CacheCluster\",\n  \"description\": \"Schema representing an Amazon ElastiCache cache cluster, which is a collection of cache nodes running Redis or Memcached cache engine software.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"CacheClusterId\"\n  ],\n  \"properties\": {\n    \"CacheClusterId\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied identifier of the cluster. This identifier is a unique key that identifies a cluster.\",\n      \"minLength\": 1,\n      \"maxLength\": 50,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9-]*$\"\n    },\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN (Amazon Resource Name) of the cache cluster.\",\n      \"pattern\": \"^arn:aws[a-zA-Z-]*:elasticache:[a-z0-9-]+:[0-9]{12}:cluster:.+$\"\n    },\n  \
  \  \"CacheClusterStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of this cluster.\",\n      \"enum\": [\n        \"available\",\n        \"creating\",\n        \"deleted\",\n        \"deleting\",\n        \"incompatible-network\",\n        \"modifying\",\n        \"rebooting cluster nodes\",\n        \"restore-failed\",\n        \"snapshotting\"\n      ]\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cache engine used in this cluster.\",\n      \"enum\": [\n        \"memcached\",\n        \"redis\"\n      ]\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the cache engine that is used in this cluster.\"\n    },\n    \"CacheNodeType\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the compute and memory capacity node type for the cluster.\",\n      \"pattern\": \"^cache\\\\.[a-z0-9]+\\\\.[a-z0-9]+$\"\n    },\n    \"NumCacheNodes\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The number of cache nodes in the cluster.\",\n      \"minimum\": 1\n    },\n    \"PreferredAvailabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Availability Zone in which the cluster is located or \\\"Multiple\\\" if the cache nodes are located in different Availability Zones.\"\n    },\n    \"CacheClusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the cluster was created.\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the weekly time range during which maintenance on the cluster is performed.\"\n    },\n    \"CacheSubnetGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cache subnet group associated with the cluster.\"\n    },\n    \"CacheParameterGroup\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Status of the cache parameter group.\",\n      \"properties\": {\n        \"CacheParameterGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the cache parameter group.\"\n        },\n        \"ParameterApplyStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of parameter updates.\"\n        },\n        \"CacheNodeIdsToReboot\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A list of the cache node IDs which need to be rebooted.\"\n        }\n      }\n    },\n    \"CacheNodes\": {\n      \"type\": \"array\",\n      \"description\": \"A list of cache nodes that are members of the cluster.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"CacheNodeId\": {\n            \"type\": \"string\",\n            \"description\": \"The cache node identifier.\"\n          },\n          \"CacheNodeStatus\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"The current state of this cache node.\"\n          },\n          \"CacheNodeCreateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time when the cache node was created.\"\n          },\n          \"Endpoint\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Address\": {\n                \"type\": \"string\",\n                \"description\": \"The DNS hostname of the cache node.\"\n              },\n              \"Port\": {\n                \"type\": \"integer\",\n                \"description\": \"The port number that the cache engine is listening on.\"\n              }\n            }\n          },\n          \"ParameterGroupStatus\": {\n            \"type\": \"string\",\n            \"description\": \"The status of the parameter group applied to this cache node.\"\n          },\n          \"CustomerAvailabilityZone\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"The Availability Zone where this node was created and now resides.\"\n          }\n        }\n      }\n    },\n    \"ConfigurationEndpoint\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a Memcached cluster endpoint which can be used by an application to connect to any node in the cluster.\",\n      \"properties\": {\n        \"Address\": {\n          \"type\": \"string\",\n          \"description\": \"The DNS hostname of the cache node.\"\n        },\n        \"Port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port number that the cache engine is listening on.\"\n        }\n      }\n    },\n    \"SecurityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"A list of VPC Security Groups associated with the cluster.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"SecurityGroupId\": {\n            \"type\": \"\
  string\",\n            \"description\": \"The identifier of the cache security group.\"\n          },\n          \"Status\": {\n            \"type\": \"string\",\n            \"description\": \"The status of the cache security group membership.\"\n          }\n        }\n      }\n    },\n    \"ReplicationGroupId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The replication group to which this cluster belongs.\"\n    },\n    \"SnapshotRetentionLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which ElastiCache retains automatic cluster snapshots.\",\n      \"minimum\": 0,\n      \"maximum\": 35\n    },\n    \"SnapshotWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The daily time range (in UTC) during which ElastiCache begins taking a daily snapshot of your cluster.\"\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, then minor version patches are\
  \ applied automatically.\",\n      \"default\": true\n    },\n    \"Port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number on which each of the cache nodes accepts connections.\"\n    },\n    \"NotificationConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a notification topic and its status.\",\n      \"properties\": {\n        \"TopicArn\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the topic.\"\n        },\n        \"TopicStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The current state of the topic.\"\n        }\n      }\n    },\n    \"TransitEncryptionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"A flag that enables in-transit encryption when set to true.\",\n      \"default\": false\n    },\n    \"AtRestEncryptionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"A flag that enables encryption\
  \ at rest when set to true.\",\n      \"default\": false\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elasticache/refs/heads/main/json-schema/amazon-elasticache-cachecluster-schema.json
tags:
- Amazon Web Services
- AWS
- Caching
- Database
- ElastiCache
- In-Memory
- Memcached
- Redis
title: Amazon ElastiCache CacheCluster
---
