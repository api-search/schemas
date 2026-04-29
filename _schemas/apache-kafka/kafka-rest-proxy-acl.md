---
description: Acl schema from Apache kafka
layout: schema
name: Acl
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
  name: resource_type
  type: string
- description: ''
  name: resource_name
  type: string
- description: ''
  name: pattern_type
  type: string
- description: ''
  name: principal
  type: string
- description: ''
  name: host
  type: string
- description: ''
  name: operation
  type: string
- description: ''
  name: permission
  type: string
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-acl-schema.json
slug: kafka-rest-proxy-acl
source_filename: kafka-rest-proxy-acl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-acl-schema.json\",\n  \"title\": \"Acl\",\n  \"description\": \"Acl schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\"\n    },\n    \"resource_type\": {\n      \"type\": \"string\"\n    },\n    \"resource_name\": {\n      \"type\": \"string\"\n    },\n    \"pattern_type\": {\n      \"type\": \"string\"\n    },\n    \"principal\": {\n      \"type\": \"string\"\n    },\n    \"host\": {\n      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"type\": \"string\"\n    },\n    \"permission\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-acl-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: Acl
---
