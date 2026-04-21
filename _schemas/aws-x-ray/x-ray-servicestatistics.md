---
description: ''
layout: schema
name: ServiceStatistics
properties_list:
- description: ''
  name: OkCount
  type: integer
- description: ''
  name: ErrorStatistics
  type: object
- description: ''
  name: FaultStatistics
  type: object
- description: ''
  name: TotalCount
  type: integer
- description: ''
  name: TotalResponseTime
  type: number
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-servicestatistics-schema.json
slug: x-ray-servicestatistics
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: ServiceStatistics
---
