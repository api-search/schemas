---
description: ''
layout: schema
name: Trace
properties_list:
- description: The unique identifier for the request that generated the trace.
  name: Id
  type: string
- description: The length of time in seconds between the start and end times.
  name: Duration
  type: number
- description: ''
  name: LimitExceeded
  type: boolean
- description: ''
  name: Segments
  type: array
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-trace-schema.json
slug: x-ray-trace
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: Trace
---
