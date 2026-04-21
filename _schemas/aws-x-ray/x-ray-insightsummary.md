---
description: ''
layout: schema
name: InsightSummary
properties_list:
- description: ''
  name: InsightId
  type: string
- description: ''
  name: GroupARN
  type: string
- description: ''
  name: GroupName
  type: string
- description: ''
  name: RootCauseServiceId
  type: object
- description: ''
  name: Categories
  type: array
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
  name: Summary
  type: string
- description: ''
  name: ClientRequestImpactStatistics
  type: object
- description: ''
  name: RootCauseServiceRequestImpactStatistics
  type: object
- description: ''
  name: TopAnomalousServices
  type: array
- description: ''
  name: LastUpdateTime
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-insightsummary-schema.json
slug: x-ray-insightsummary
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: InsightSummary
---
