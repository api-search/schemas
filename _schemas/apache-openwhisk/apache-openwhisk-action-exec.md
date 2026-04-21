---
description: ActionExec schema from Apache OpenWhisk
layout: schema
name: ActionExec
properties_list:
- description: Runtime kind
  name: kind
  type: string
- description: Inline function source code
  name: code
  type: string
- description: Docker image for blackbox/docker kind
  name: image
  type: string
- description: Sequence of action names (for sequence kind)
  name: components
  type: array
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-action-exec-schema.json
slug: apache-openwhisk-action-exec
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActionExec
---
