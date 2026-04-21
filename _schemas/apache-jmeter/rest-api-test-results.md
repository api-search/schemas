---
description: Test performance results
layout: schema
name: TestResults
properties_list:
- description: ''
  name: testId
  type: string
- description: ''
  name: totalRequests
  type: integer
- description: ''
  name: errorCount
  type: integer
- description: Average response time in milliseconds
  name: averageResponseTime
  type: number
- description: ''
  name: minResponseTime
  type: number
- description: ''
  name: maxResponseTime
  type: number
- description: 90th percentile response time
  name: percentile90
  type: number
- description: Average throughput in requests/second
  name: throughput
  type: number
provider_name: Apache JMeter
provider_slug: apache-jmeter
schema_file: json-schema/rest-api-test-results-schema.json
slug: rest-api-test-results
tags:
- API Testing
- Java
- Load Testing
- Open Source
- Performance Testing
- Stress Testing
title: TestResults
---
