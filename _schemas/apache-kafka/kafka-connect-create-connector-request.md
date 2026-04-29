---
description: CreateConnectorRequest schema from Apache kafka
layout: schema
name: CreateConnectorRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: config
  type: object
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-connect-create-connector-request-schema.json
slug: kafka-connect-create-connector-request
source_filename: kafka-connect-create-connector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-create-connector-request-schema.json\",\n  \"title\": \"CreateConnectorRequest\",\n  \"description\": \"CreateConnectorRequest schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"config\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-create-connector-request-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: CreateConnectorRequest
---
