---
description: ClusterData schema from Apache Pulsar
layout: schema
name: ClusterData
properties_list:
- description: ''
  name: serviceUrl
  type: string
- description: ''
  name: serviceUrlTls
  type: string
- description: ''
  name: brokerServiceUrl
  type: string
- description: ''
  name: brokerServiceUrlTls
  type: string
- description: ''
  name: peerClusterNames
  type: array
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-cluster-data-schema.json
slug: apache-pulsar-cluster-data
source_filename: apache-pulsar-cluster-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-cluster-data-schema.json\",\n  \"title\": \"ClusterData\",\n  \"description\": \"ClusterData schema from Apache Pulsar\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceUrl\": {\n      \"type\": \"string\"\n    },\n    \"serviceUrlTls\": {\n      \"type\": \"string\"\n    },\n    \"brokerServiceUrl\": {\n      \"type\": \"string\"\n    },\n    \"brokerServiceUrlTls\": {\n      \"type\": \"string\"\n    },\n    \"peerClusterNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-cluster-data-schema.json
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: ClusterData
---
