---
description: Standard Jolokia response envelope for successful MBean read operations.
layout: schema
name: JolokiaResponse
properties_list:
- description: Echo of the original request details.
  name: request
  type: object
- description: The attribute value returned. Type varies by attribute.
  name: value
  type: object
- description: Unix timestamp of the response.
  name: timestamp
  type: integer
- description: HTTP status code of the Jolokia operation.
  name: status
  type: integer
provider_name: Apache ActiveMQ
provider_slug: apache-activemq
schema_file: json-schema/rest-jolokia-response-schema.json
slug: rest-jolokia-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-activemq/refs/heads/main/json-schema/rest-jolokia-response-schema.json\",\n  \"title\": \"JolokiaResponse\",\n  \"description\": \"Standard Jolokia response envelope for successful MBean read operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request\": {\n      \"type\": \"object\",\n      \"description\": \"Echo of the original request details.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Jolokia operation type (read, write, exec, search).\",\n          \"example\": \"read\"\n        },\n        \"mbean\": {\n          \"type\": \"string\",\n          \"description\": \"JMX ObjectName of the target MBean.\",\n          \"example\": \"org.apache.activemq:type=Broker,brokerName=localhost\"\n        },\n        \"attribute\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Attribute name that was read.\",\n          \"example\": \"TotalConsumerCount\"\n        }\n      }\n    },\n    \"value\": {\n      \"description\": \"The attribute value returned. Type varies by attribute.\",\n      \"example\": 3\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the response.\",\n      \"example\": 1718153645\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code of the Jolokia operation.\",\n      \"example\": 200\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-activemq/refs/heads/main/json-schema/rest-jolokia-response-schema.json
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
title: JolokiaResponse
---
