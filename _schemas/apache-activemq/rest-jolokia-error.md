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
