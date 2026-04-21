---
description: Current test status
layout: schema
name: TestStatus
properties_list:
- description: ''
  name: testId
  type: string
- description: ''
  name: status
  type: string
- description: Number of active virtual user threads
  name: activeThreads
  type: integer
- description: Elapsed test time in milliseconds
  name: elapsedTime
  type: integer
- description: Current throughput in requests per second
  name: throughput
  type: number
- description: Current error rate percentage
  name: errorRate
  type: number
provider_name: Apache JMeter
provider_slug: apache-jmeter
schema_file: json-schema/rest-api-test-status-schema.json
slug: rest-api-test-status
tags:
- API Testing
- Java
- Load Testing
- Open Source
- Performance Testing
- Stress Testing
title: TestStatus
---
