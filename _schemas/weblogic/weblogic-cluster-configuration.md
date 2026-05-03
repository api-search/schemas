---
description: Configuration schema for an Oracle WebLogic Server cluster including messaging mode, load balancing algorithm, and multicast settings.
layout: schema
name: WebLogic Cluster Configuration
properties_list:
- description: Unique name of the cluster within the domain
  name: name
  type: string
- description: Messaging mode used for cluster communication
  name: clusterMessagingMode
  type: string
- description: Multicast channel name for cluster communication (used with multicast mode)
  name: clusterBroadcastChannel
  type: string
- description: Multicast address for cluster heartbeat messages
  name: multicastAddress
  type: string
- description: Multicast port for cluster heartbeat messages
  name: multicastPort
  type: integer
- description: Comma-separated list of host:port pairs for all servers in the cluster
  name: clusterAddress
  type: string
- description: Load balancing algorithm for routing requests to cluster members
  name: defaultLoadAlgorithm
  type: string
- description: Whether the WebLogic plugin is enabled for this cluster
  name: weblogicPluginEnabled
  type: boolean
- description: Frontend hostname for the cluster (used in URL generation behind a load balancer)
  name: frontendHost
  type: string
- description: Frontend HTTP port
  name: frontendHTTPPort
  type: integer
- description: Frontend HTTPS port
  name: frontendHTTPSPort
  type: integer
- description: Number of HTTP ping retries before marking a server as failed
  name: httpPingRetryCount
  type: integer
- description: Period in seconds between HTTP health pings
  name: httpPingPeriod
  type: integer
- description: Basis for automatic service migration
  name: migrationBasis
  type: string
- description: Data source used for database-based automatic migration leasing
  name: dataSourceForAutomaticMigration
  type: string
- description: Network channel used for session replication
  name: replicationChannel
  type: string
- description: Interval in seconds for flushing session data to the replication channel
  name: sessionFlushInterval
  type: integer
- description: Number of servers to include in the generated cluster address
  name: numberOfServersInClusterAddress
  type: integer
provider_name: Oracle WebLogic Server APIs
provider_slug: weblogic
schema_file: json-schema/weblogic-cluster-configuration.json
slug: weblogic-cluster-configuration
source_filename: weblogic-cluster-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/weblogic/cluster-configuration\",\n  \"title\": \"WebLogic Cluster Configuration\",\n  \"description\": \"Configuration schema for an Oracle WebLogic Server cluster including messaging mode, load balancing algorithm, and multicast settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the cluster within the domain\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"clusterMessagingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Messaging mode used for cluster communication\",\n      \"enum\": [\"unicast\", \"multicast\"],\n      \"default\": \"unicast\"\n    },\n    \"clusterBroadcastChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Multicast channel name for cluster communication (used with multicast mode)\"\n    },\n    \"multicastAddress\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Multicast address for cluster heartbeat messages\",\n      \"default\": \"239.192.0.0\"\n    },\n    \"multicastPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Multicast port for cluster heartbeat messages\",\n      \"default\": 7001,\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"clusterAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of host:port pairs for all servers in the cluster\"\n    },\n    \"defaultLoadAlgorithm\": {\n      \"type\": \"string\",\n      \"description\": \"Load balancing algorithm for routing requests to cluster members\",\n      \"enum\": [\n        \"round-robin\",\n        \"weight-based\",\n        \"round-robin-affinity\",\n        \"weight-based-affinity\",\n        \"random\"\n      ],\n      \"default\": \"round-robin\"\n    },\n    \"weblogicPluginEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the WebLogic plugin is enabled for this cluster\",\n      \"default\": false\n    },\n    \"frontendHost\": {\n      \"type\": \"string\",\n      \"description\": \"Frontend hostname for the cluster (used in URL generation behind a load balancer)\"\n    },\n    \"frontendHTTPPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Frontend HTTP port\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"frontendHTTPSPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Frontend HTTPS port\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"httpPingRetryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of HTTP ping retries before marking a server as failed\",\n      \"default\": 3,\n      \"minimum\": 0\n    },\n    \"httpPingPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Period in seconds between HTTP health pings\",\n      \"default\": 10,\n      \"minimum\": 1\n    },\n    \"migrationBasis\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Basis for automatic service migration\",\n      \"enum\": [\"consensus\", \"database\"],\n      \"default\": \"consensus\"\n    },\n    \"dataSourceForAutomaticMigration\": {\n      \"type\": \"string\",\n      \"description\": \"Data source used for database-based automatic migration leasing\"\n    },\n    \"replicationChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Network channel used for session replication\"\n    },\n    \"sessionFlushInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Interval in seconds for flushing session data to the replication channel\",\n      \"default\": 3\n    },\n    \"numberOfServersInClusterAddress\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of servers to include in the generated cluster address\",\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/json-schema/weblogic-cluster-configuration.json
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
- WebLogic
title: WebLogic Cluster Configuration
---
