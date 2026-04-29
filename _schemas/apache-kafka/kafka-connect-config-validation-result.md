---
description: ConfigValidationResult schema from Apache kafka
layout: schema
name: ConfigValidationResult
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: error_count
  type: integer
- description: ''
  name: groups
  type: array
- description: ''
  name: configs
  type: array
provider_name: Apache Kafka
provider_slug: apache-kafka
schema_file: json-schema/kafka-connect-config-validation-result-schema.json
slug: kafka-connect-config-validation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-config-validation-result-schema.json\",\n  \"title\": \"ConfigValidationResult\",\n  \"description\": \"ConfigValidationResult schema from Apache kafka\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"error_count\": {\n      \"type\": \"integer\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"configs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kafka/refs/heads/main/json-schema/kafka-connect-config-validation-result-schema.json
tags:
- Distributed Systems
- Event Streaming
- Messaging
- Open Source
- Pub-Sub
title: ConfigValidationResult
---
