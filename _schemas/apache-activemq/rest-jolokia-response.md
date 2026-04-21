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
