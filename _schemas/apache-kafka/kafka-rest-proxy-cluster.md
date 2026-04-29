---
description: Cluster schema from Apache kafka
layout: schema
name: Cluster
properties_list:
- description: ''
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: cluster_id
  type: string
- description: ''
  name: controller
  type: object
- description: ''
  name: brokers
  type: object
- description: ''
  name: topics
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-cluster-schema.json
slug: kafka-rest-proxy-cluster
source_filename: kafka-rest-proxy-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"Cluster schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\"\n        },\n        \"resource_name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"controller\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"related\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"brokers\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"related\": {\n          \"type\": \"string\"\n        }\n\
  \      }\n    },\n    \"topics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"related\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-cluster-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Cluster
---
