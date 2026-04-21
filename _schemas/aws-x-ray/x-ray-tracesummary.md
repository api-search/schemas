---
description: ''
layout: schema
name: TraceSummary
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Duration
  type: number
- description: ''
  name: ResponseTime
  type: number
- description: ''
  name: HasFault
  type: boolean
- description: ''
  name: HasError
  type: boolean
- description: ''
  name: HasThrottle
  type: boolean
- description: ''
  name: IsPartial
  type: boolean
- description: ''
  name: Http
  type: object
- description: ''
  name: Annotations
  type: object
- description: ''
  name: Users
  type: array
- description: ''
  name: ServiceIds
  type: array
- description: ''
  name: EntryPoint
  type: object
- description: ''
  name: MatchedEventTime
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-tracesummary-schema.json
slug: x-ray-tracesummary
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: TraceSummary
---
