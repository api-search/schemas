---
description: Represents a cluster of IBM WebSphere Application Server instances or Liberty collective members that work together to provide high availability, workload distribution, and failover capabilities.
layout: schema
name: WebSphere Cluster
properties_list:
- description: The unique name of the cluster.
  name: name
  type: string
- description: Human-readable display name for the cluster.
  name: displayName
  type: string
- description: Description of the cluster purpose and configuration.
  name: description
  type: string
- description: Overall cluster status based on member states.
  name: status
  type: string
- description: Type of cluster.
  name: clusterType
  type: string
- description: Name of the cell this cluster belongs to.
  name: cellName
  type: string
- description: Server instances that are members of this cluster.
  name: members
  type: array
- description: Total number of members in the cluster.
  name: memberCount
  type: integer
- description: Number of currently running members.
  name: membersStarted
  type: integer
- description: Whether to prefer routing requests to local cluster members.
  name: preferLocal
  type: boolean
- description: Load balancing configuration for the cluster.
  name: loadBalancingPolicy
  type: object
- description: Auto-scaling policy for the cluster.
  name: scalingPolicy
  type: object
- description: Service policy configuration.
  name: servicePolicy
  type: object
- description: Data replication configuration for the cluster.
  name: replicationDomain
  type: object
- description: Applications deployed to this cluster.
  name: applications
  type: array
- description: Date and time the cluster was created.
  name: createdDate
  type: string
- description: Date and time the cluster was last modified.
  name: lastModified
  type: string
- description: Additional metadata associated with the cluster.
  name: metadata
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/cluster.json
slug: cluster
source_json: "{\n  \"$id\": \"cluster.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSphere Cluster\",\n  \"description\": \"Represents a cluster of IBM WebSphere Application Server instances or Liberty collective members that work together to provide high availability, workload distribution, and failover capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the cluster.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the cluster.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the cluster purpose and configuration.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"running\", \"stopped\", \"partial\", \"unknown\"],\n      \"description\": \"Overall cluster status based on member states.\"\n\
  \    },\n    \"clusterType\": {\n      \"type\": \"string\",\n      \"enum\": [\"APPLICATION_SERVER\", \"PROXY_SERVER\", \"LIBERTY_COLLECTIVE\"],\n      \"description\": \"Type of cluster.\"\n    },\n    \"cellName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cell this cluster belongs to.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Server instances that are members of this cluster.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"serverName\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the member server.\"\n          },\n          \"nodeName\": {\n            \"type\": \"string\",\n            \"description\": \"Node where the member resides.\"\n          },\n          \"hostName\": {\n            \"type\": \"string\",\n            \"description\": \"Hostname of the member.\"\n          },\n          \"status\": {\n            \"type\": \"string\"\
  ,\n            \"enum\": [\"STARTED\", \"STOPPED\", \"STARTING\", \"STOPPING\", \"UNKNOWN\"],\n            \"description\": \"Current status of the cluster member.\"\n          },\n          \"weight\": {\n            \"type\": \"integer\",\n            \"minimum\": 0,\n            \"maximum\": 20,\n            \"default\": 2,\n            \"description\": \"Workload management weight for this member.\"\n          },\n          \"uniqueId\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the cluster member.\"\n          }\n        },\n        \"required\": [\"serverName\"]\n      }\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of members in the cluster.\"\n    },\n    \"membersStarted\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently running members.\"\n    },\n    \"preferLocal\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\"\
  : \"Whether to prefer routing requests to local cluster members.\"\n    },\n    \"loadBalancingPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Load balancing configuration for the cluster.\",\n      \"properties\": {\n        \"policy\": {\n          \"type\": \"string\",\n          \"enum\": [\"ROUND_ROBIN\", \"WEIGHTED\", \"RANDOM\"],\n          \"description\": \"Load balancing algorithm.\"\n        },\n        \"stickySession\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether to enable session affinity.\"\n        }\n      }\n    },\n    \"scalingPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Auto-scaling policy for the cluster.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether auto-scaling is enabled.\"\n        },\n        \"minMembers\": {\n          \"type\": \"integer\",\n       \
  \   \"minimum\": 1,\n          \"description\": \"Minimum number of cluster members.\"\n        },\n        \"maxMembers\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of cluster members.\"\n        },\n        \"scaleUpThreshold\": {\n          \"type\": \"number\",\n          \"description\": \"CPU or memory utilization percentage to trigger scale-up.\"\n        },\n        \"scaleDownThreshold\": {\n          \"type\": \"number\",\n          \"description\": \"CPU or memory utilization percentage to trigger scale-down.\"\n        },\n        \"cooldownPeriod\": {\n          \"type\": \"integer\",\n          \"description\": \"Cooldown period in seconds between scaling events.\"\n        }\n      }\n    },\n    \"servicePolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Service policy configuration.\",\n      \"properties\": {\n        \"matchCriteria\": {\n          \"type\": \"string\",\n          \"description\": \"Criteria for\
  \ matching requests to this cluster.\"\n        },\n        \"priority\": {\n          \"type\": \"integer\",\n          \"description\": \"Priority of this service policy.\"\n        }\n      }\n    },\n    \"replicationDomain\": {\n      \"type\": \"object\",\n      \"description\": \"Data replication configuration for the cluster.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Replication domain name.\"\n        },\n        \"numberOfReplicas\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of replicas for session data.\"\n        },\n        \"requestTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Replication request timeout in seconds.\"\n        }\n      }\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"description\": \"Applications deployed to this cluster.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the cluster was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the cluster was last modified.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Additional metadata associated with the cluster.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/cluster.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: WebSphere Cluster
---
