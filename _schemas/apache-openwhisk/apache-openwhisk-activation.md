---
description: Activation schema from Apache OpenWhisk
layout: schema
name: Activation
properties_list:
- description: Unique activation identifier
  name: activationId
  type: string
- description: ''
  name: namespace
  type: string
- description: Name of invoked action/trigger
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: Subject who invoked the action
  name: subject
  type: string
- description: Start time epoch ms
  name: start
  type: integer
- description: End time epoch ms
  name: end
  type: integer
- description: Duration in milliseconds
  name: duration
  type: integer
- description: ''
  name: response
  type: object
- description: Activation log output
  name: logs
  type: array
- description: ''
  name: annotations
  type: array
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-activation-schema.json
slug: apache-openwhisk-activation
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: Activation
---
