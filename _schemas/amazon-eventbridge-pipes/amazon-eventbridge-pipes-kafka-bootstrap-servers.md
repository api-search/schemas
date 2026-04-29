---
description: KafkaBootstrapServers schema from Amazon EventBridge Pipes
layout: schema
name: KafkaBootstrapServers
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-kafka-bootstrap-servers-schema.json
slug: amazon-eventbridge-pipes-kafka-bootstrap-servers
source_filename: amazon-eventbridge-pipes-kafka-bootstrap-servers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-kafka-bootstrap-servers-schema.json\",\n  \"title\": \"KafkaBootstrapServers\",\n  \"description\": \"KafkaBootstrapServers schema from Amazon EventBridge Pipes\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/EndpointString\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 2\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-kafka-bootstrap-servers-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: KafkaBootstrapServers
---
