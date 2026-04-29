---
description: Schema representing a Couchbase cluster including nodes, services, server groups, and configuration settings.
layout: schema
name: Couchbase Cluster Configuration
properties_list:
- description: Human-readable name for the cluster
  name: name
  type: string
- description: Unique identifier for the cluster
  name: uuid
  type: string
- description: List of nodes in the cluster
  name: nodes
  type: array
- description: Server groups for rack-zone awareness
  name: serverGroups
  type: array
- description: RAM quota allocations per service in megabytes
  name: ramQuota
  type: object
- description: ''
  name: autoCompaction
  type: object
- description: ''
  name: autoFailover
  type: object
provider_name: Couchbase
provider_slug: couchbase
schema_file: json-schema/couchbase-cluster-schema.json
slug: couchbase-cluster
source_filename: couchbase-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://couchbase.com/schemas/couchbase/cluster.json\",\n  \"title\": \"Couchbase Cluster Configuration\",\n  \"description\": \"Schema representing a Couchbase cluster including nodes, services, server groups, and configuration settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the cluster\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the cluster\"\n    },\n    \"nodes\": {\n      \"type\": \"array\",\n      \"description\": \"List of nodes in the cluster\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Node\"\n      }\n    },\n    \"serverGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Server groups for rack-zone awareness\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ServerGroup\"\n      }\n    },\n    \"\
  ramQuota\": {\n      \"type\": \"object\",\n      \"description\": \"RAM quota allocations per service in megabytes\",\n      \"properties\": {\n        \"dataService\": {\n          \"type\": \"integer\",\n          \"description\": \"RAM quota for the Data service in megabytes\",\n          \"minimum\": 256\n        },\n        \"indexService\": {\n          \"type\": \"integer\",\n          \"description\": \"RAM quota for the Index service in megabytes\",\n          \"minimum\": 256\n        },\n        \"searchService\": {\n          \"type\": \"integer\",\n          \"description\": \"RAM quota for the Search service in megabytes\",\n          \"minimum\": 256\n        },\n        \"analyticsService\": {\n          \"type\": \"integer\",\n          \"description\": \"RAM quota for the Analytics service in megabytes\",\n          \"minimum\": 1024\n        },\n        \"eventingService\": {\n          \"type\": \"integer\",\n          \"description\": \"RAM quota for the Eventing\
  \ service in megabytes\",\n          \"minimum\": 256\n        }\n      }\n    },\n    \"autoCompaction\": {\n      \"$ref\": \"#/$defs/AutoCompactionSettings\"\n    },\n    \"autoFailover\": {\n      \"$ref\": \"#/$defs/AutoFailoverSettings\"\n    }\n  },\n  \"$defs\": {\n    \"Node\": {\n      \"type\": \"object\",\n      \"description\": \"A node in the Couchbase cluster\",\n      \"required\": [\n        \"hostname\"\n      ],\n      \"properties\": {\n        \"hostname\": {\n          \"type\": \"string\",\n          \"description\": \"Hostname or IP address with port\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Health status of the node\",\n          \"enum\": [\n            \"healthy\",\n            \"unhealthy\",\n            \"warmup\"\n          ]\n        },\n        \"clusterMembership\": {\n          \"type\": \"string\",\n          \"description\": \"Cluster membership state of the node\",\n          \"enum\": [\n  \
  \          \"active\",\n            \"inactiveAdded\",\n            \"inactiveFailed\"\n          ]\n        },\n        \"services\": {\n          \"type\": \"array\",\n          \"description\": \"Services running on the node\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"kv\",\n              \"n1ql\",\n              \"index\",\n              \"fts\",\n              \"cbas\",\n              \"eventing\",\n              \"backup\"\n            ]\n          },\n          \"minItems\": 1\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Couchbase Server version installed on the node\"\n        },\n        \"os\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system of the node\"\n        },\n        \"cpuCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of CPU cores on the node\",\n          \"minimum\": 1\n        },\n  \
  \      \"memoryTotal\": {\n          \"type\": \"integer\",\n          \"description\": \"Total memory on the node in bytes\"\n        },\n        \"memoryFree\": {\n          \"type\": \"integer\",\n          \"description\": \"Free memory on the node in bytes\"\n        },\n        \"addressFamily\": {\n          \"type\": \"string\",\n          \"description\": \"Network address family\",\n          \"enum\": [\n            \"inet\",\n            \"inet6\",\n            \"inet6only\"\n          ]\n        },\n        \"nodeEncryption\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether node-to-node encryption is enabled\"\n        }\n      }\n    },\n    \"ServerGroup\": {\n      \"type\": \"object\",\n      \"description\": \"A server group for rack-zone awareness\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the server group\"\n     \
  \   },\n        \"uri\": {\n          \"type\": \"string\",\n          \"description\": \"URI path to the server group resource\"\n        },\n        \"nodes\": {\n          \"type\": \"array\",\n          \"description\": \"Nodes assigned to this server group\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Node\"\n          }\n        }\n      }\n    },\n    \"AutoCompactionSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Auto-compaction settings for the cluster\",\n      \"properties\": {\n        \"databaseFragmentationThreshold\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"percentage\": {\n              \"type\": \"integer\",\n              \"description\": \"Fragmentation percentage trigger\",\n              \"minimum\": 2,\n              \"maximum\": 100\n            },\n            \"size\": {\n              \"type\": \"integer\",\n              \"description\": \"Fragmentation size trigger in bytes\",\n      \
  \        \"minimum\": 1048576\n            }\n          }\n        },\n        \"viewFragmentationThreshold\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"percentage\": {\n              \"type\": \"integer\",\n              \"description\": \"View fragmentation percentage trigger\",\n              \"minimum\": 2,\n              \"maximum\": 100\n            },\n            \"size\": {\n              \"type\": \"integer\",\n              \"description\": \"View fragmentation size trigger in bytes\",\n              \"minimum\": 1048576\n            }\n          }\n        },\n        \"parallelDBAndViewCompaction\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to run database and view compaction in parallel\"\n        },\n        \"allowedTimePeriod\": {\n          \"type\": \"object\",\n          \"description\": \"Time window during which compaction is allowed\",\n          \"properties\": {\n            \"fromHour\": {\n\
  \              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"maximum\": 23\n            },\n            \"fromMinute\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"maximum\": 59\n            },\n            \"toHour\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"maximum\": 23\n            },\n            \"toMinute\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"maximum\": 59\n            },\n            \"abortOutside\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether to abort compaction outside the time window\"\n            }\n          }\n        }\n      }\n    },\n    \"AutoFailoverSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Auto-failover settings for the cluster\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Whether auto-failover is enabled\"\n        },\n        \"timeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of seconds to wait before auto-failover triggers\",\n          \"minimum\": 5,\n          \"maximum\": 3600\n        },\n        \"maxCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of auto-failovers before requiring manual reset\",\n          \"minimum\": 1\n        },\n        \"failoverOnDataDiskIssues\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether to failover on data disk issues\"\n            },\n            \"timePeriod\": {\n              \"type\": \"integer\",\n              \"description\": \"Time period in seconds to wait for disk issue resolution\",\n              \"minimum\": 5\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/json-schema/couchbase-cluster-schema.json
tags:
- Analytics
- App Services
- Backup
- Capella
- Cloud
- Database
- DBaaS
- Eventing
- Full-Text Search
- Gateway
- JSON
- Mobile
- NoSQL
- Replication
- SQL++
- Sync
- Vector Search
- XDCR
title: Couchbase Cluster Configuration
---
