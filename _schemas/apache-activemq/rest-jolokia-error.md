---
description: Jolokia error response envelope.
layout: schema
name: JolokiaError
properties_list:
- description: Error class name.
  name: error_type
  type: string
- description: Error message.
  name: error
  type: string
- description: HTTP status code.
  name: status
  type: integer
- description: Unix timestamp of the error response.
  name: timestamp
  type: integer
provider_name: Apache ActiveMQ
provider_slug: apache-activemq
schema_file: json-schema/rest-jolokia-error-schema.json
slug: rest-jolokia-error
source_filename: rest-jolokia-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-activemq/refs/heads/main/json-schema/rest-jolokia-error-schema.json\",\n  \"title\": \"JolokiaError\",\n  \"description\": \"Jolokia error response envelope.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error_type\": {\n      \"type\": \"string\",\n      \"description\": \"Error class name.\",\n      \"example\": \"java.lang.IllegalArgumentException\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message.\",\n      \"example\": \"No MBean found for pattern\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 404\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the error response.\",\n      \"example\": 1718153645\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-activemq/refs/heads/main/json-schema/rest-jolokia-error-schema.json
tags:
- AMQP
- Apache
- Java
- JMS
- Message Broker
- Messaging
- MQTT
- Open Source
- STOMP
title: JolokiaError
---
