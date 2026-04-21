---
description: ''
layout: schema
name: Service
properties_list:
- description: ''
  name: ReferenceId
  type: integer
- description: ''
  name: Name
  type: string
- description: ''
  name: Names
  type: array
- description: ''
  name: Root
  type: boolean
- description: ''
  name: AccountId
  type: string
- description: ''
  name: Type
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: StartTime
  type: string
- description: ''
  name: EndTime
  type: string
- description: ''
  name: Edges
  type: array
- description: ''
  name: SummaryStatistics
  type: object
- description: ''
  name: ResponseTimeHistogram
  type: array
- description: ''
  name: DurationHistogram
  type: array
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-service-schema.json
slug: x-ray-service
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: Service
---
