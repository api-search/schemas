---
description: ClusterInfo schema from Apache Pinot
layout: schema
name: ClusterInfo
properties_list:
- description: ''
  name: clusterName
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: numOnlineControllers
  type: integer
- description: ''
  name: numOnlineBrokers
  type: integer
- description: ''
  name: numOnlineServers
  type: integer
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-cluster-info-schema.json
slug: apache-pinot-cluster-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-cluster-info-schema.json\",\n  \"title\": \"ClusterInfo\",\n  \"description\": \"ClusterInfo schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"example\": \"PinotCluster\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"1.0.0\"\n    },\n    \"numOnlineControllers\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"numOnlineBrokers\": {\n      \"type\": \"integer\",\n      \"example\": 2\n    },\n    \"numOnlineServers\": {\n      \"type\": \"integer\",\n      \"example\": 4\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-cluster-info-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: ClusterInfo
---
