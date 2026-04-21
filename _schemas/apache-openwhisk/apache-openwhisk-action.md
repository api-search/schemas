---
description: Action schema from Apache OpenWhisk
layout: schema
name: Action
properties_list:
- description: Namespace owning the action
  name: namespace
  type: string
- description: Action name
  name: name
  type: string
- description: Action version
  name: version
  type: string
- description: Whether the action is public
  name: publish
  type: boolean
- description: ''
  name: exec
  type: object
- description: ''
  name: annotations
  type: array
- description: ''
  name: parameters
  type: array
- description: ''
  name: limits
  type: object
- description: Last update timestamp (epoch ms)
  name: updated
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-action-schema.json
slug: apache-openwhisk-action
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: Action
---
