---
description: Cluster schema from Veritas InfoScale REST API
layout: schema
name: Cluster
properties_list:
- description: Unique cluster identifier
  name: clusterId
  type: string
- description: Name of the cluster
  name: clusterName
  type: string
- description: Current cluster state
  name: state
  type: string
- description: Number of nodes in the cluster
  name: nodeCount
  type: integer
- description: InfoScale cluster version
  name: clusterVersion
  type: string
- description: I/O fencing mode
  name: fencingMode
  type: string
- description: Cluster uptime duration
  name: uptime
  type: string
- description: Last configuration change timestamp
  name: lastModified
  type: string
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
schema_file: json-schema/rest-api-cluster-schema.json
slug: rest-api-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"Cluster schema from Veritas InfoScale REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cluster identifier\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cluster\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"RUNNING\", \"FAULTED\", \"PARTIAL\", \"OFFLINE\"],\n      \"description\": \"Current cluster state\"\n    },\n    \"nodeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of nodes in the cluster\"\n    },\n    \"clusterVersion\": {\n      \"type\": \"string\",\n      \"description\": \"InfoScale cluster version\"\n    },\n\
  \    \"fencingMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"scsi3\", \"customized\", \"disabled\"],\n      \"description\": \"I/O fencing mode\"\n    },\n    \"uptime\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster uptime duration\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last configuration change timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-cluster-schema.json
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
title: Cluster
---
