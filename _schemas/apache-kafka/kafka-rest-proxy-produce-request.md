---
description: ProduceRequest schema from Apache kafka
layout: schema
name: ProduceRequest
properties_list:
- description: ''
  name: partition_id
  type: integer
- description: ''
  name: headers
  type: array
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-rest-proxy-produce-request-schema.json
slug: kafka-rest-proxy-produce-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-produce-request-schema.json\",\n  \"title\": \"ProduceRequest\",\n  \"description\": \"ProduceRequest schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partition_id\": {\n      \"type\": \"integer\"\n    },\n    \"headers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"key\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"BINARY\",\n            \"JSON\",\n            \"AVRO\",\n            \"PROTOBUF\",\n            \"JSONSCHEMA\"\
  \n          ]\n        },\n        \"data\": {}\n      }\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"BINARY\",\n            \"JSON\",\n            \"AVRO\",\n            \"PROTOBUF\",\n            \"JSONSCHEMA\"\n          ]\n        },\n        \"data\": {}\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-rest-proxy-produce-request-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: ProduceRequest
---
