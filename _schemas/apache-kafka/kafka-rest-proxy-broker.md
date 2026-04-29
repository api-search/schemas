---
description: Broker schema from Apache kafka
layout: schema
name: Broker
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
  name: broker_id
  type: integer
- description: ''
  name: host
  type: string
- description: ''
  name: port
  type: integer
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-broker-schema.json
slug: kafka-rest-proxy-broker
source_filename: kafka-rest-proxy-broker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-broker-schema.json\",\n  \"title\": \"Broker\",\n  \"description\": \"Broker schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"broker_id\": {\n      \"type\": \"integer\"\n    },\n    \"host\": {\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-broker-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Broker
---
