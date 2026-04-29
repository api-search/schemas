---
description: CacheCluster schema from Amazon ElastiCache API
layout: schema
name: CacheCluster
properties_list:
- description: The user-supplied identifier of the cluster.
  name: CacheClusterId
  type: string
- description: The current state of this cluster.
  name: CacheClusterStatus
  type: string
- description: The name of the cache engine used for this cluster.
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
- description: The name of the Availability Zone in which the cluster is located.
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
- description: A list of cache nodes that are members of the cluster.
  name: CacheNodes
  type: array
- description: If true, then minor version patches are applied automatically.
  name: AutoMinorVersionUpgrade
  type: boolean
- description: A list of VPC Security Groups associated with the cluster.
  name: SecurityGroups
  type: array
- description: The replication group to which this cluster belongs.
  name: ReplicationGroupId
  type: string
- description: The number of days for which ElastiCache retains automatic cluster snapshots.
  name: SnapshotRetentionLimit
  type: integer
- description: The ARN of the cache cluster.
  name: ARN
  type: string
provider_name: Amazon ElastiCache
provider_slug: amazon-elasticache
schema_file: json-schema/amazon-elasticache-cache-cluster-schema.json
slug: amazon-elasticache-cache-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elasticache/refs/heads/main/json-schema/amazon-elasticache-cache-cluster-schema.json\",\n  \"title\": \"CacheCluster\",\n  \"description\": \"CacheCluster schema from Amazon ElastiCache API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CacheClusterId\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied identifier of the cluster.\"\n    },\n    \"CacheClusterStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of this cluster.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cache engine used for this cluster.\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the cache engine that is used in this cluster.\"\n    },\n    \"CacheNodeType\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The name of the compute and memory capacity node type for the cluster.\"\n    },\n    \"NumCacheNodes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of cache nodes in the cluster.\"\n    },\n    \"PreferredAvailabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Availability Zone in which the cluster is located.\"\n    },\n    \"CacheClusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the cluster was created.\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the weekly time range during which maintenance on the cluster is performed.\"\n    },\n    \"CacheSubnetGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cache subnet group associated with the cluster.\"\n    },\n    \"CacheNodes\": {\n      \"type\": \"array\",\n\
  \      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"CacheNodeId\": {\n            \"type\": \"string\"\n          },\n          \"CacheNodeStatus\": {\n            \"type\": \"string\"\n          },\n          \"Endpoint\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Address\": {\n                \"type\": \"string\"\n              },\n              \"Port\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      },\n      \"description\": \"A list of cache nodes that are members of the cluster.\"\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, then minor version patches are applied automatically.\"\n    },\n    \"SecurityGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"SecurityGroupId\": {\n            \"type\": \"string\"\
  \n          },\n          \"Status\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"A list of VPC Security Groups associated with the cluster.\"\n    },\n    \"ReplicationGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"The replication group to which this cluster belongs.\"\n    },\n    \"SnapshotRetentionLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which ElastiCache retains automatic cluster snapshots.\"\n    },\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the cache cluster.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elasticache/refs/heads/main/json-schema/amazon-elasticache-cache-cluster-schema.json
tags:
- Amazon Web Services
- AWS
- Caching
- Database
- ElastiCache
- In-Memory
- Memcached
- Redis
title: CacheCluster
---
