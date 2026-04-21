---
description: ''
layout: schema
name: SamplingRule
properties_list:
- description: ''
  name: RuleName
  type: string
- description: ''
  name: RuleARN
  type: string
- description: ''
  name: ResourceARN
  type: string
- description: ''
  name: Priority
  type: integer
- description: ''
  name: FixedRate
  type: number
- description: ''
  name: ReservoirSize
  type: integer
- description: ''
  name: ServiceName
  type: string
- description: ''
  name: ServiceType
  type: string
- description: ''
  name: Host
  type: string
- description: ''
  name: HTTPMethod
  type: string
- description: ''
  name: URLPath
  type: string
- description: ''
  name: Version
  type: integer
- description: ''
  name: Attributes
  type: object
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-samplingrule-schema.json
slug: x-ray-samplingrule
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: SamplingRule
---
