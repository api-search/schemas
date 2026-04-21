---
description: FunctionConfig schema from Apache Pulsar
layout: schema
name: FunctionConfig
properties_list:
- description: ''
  name: tenant
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: className
  type: string
- description: ''
  name: inputs
  type: array
- description: ''
  name: output
  type: string
- description: ''
  name: logTopic
  type: string
- description: ''
  name: processingGuarantees
  type: string
- description: ''
  name: parallelism
  type: integer
- description: ''
  name: runtime
  type: string
- description: ''
  name: autoAck
  type: boolean
- description: ''
  name: userConfig
  type: object
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-function-config-schema.json
slug: apache-pulsar-function-config
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: FunctionConfig
---
