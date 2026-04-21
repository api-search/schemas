---
description: Request to start a JMeter test
layout: schema
name: TestRunRequest
properties_list:
- description: Path to the JMeter test plan file
  name: testPlan
  type: string
- description: JMeter properties to override
  name: properties
  type: object
provider_name: Apache JMeter
provider_slug: apache-jmeter
schema_file: json-schema/rest-api-test-run-request-schema.json
slug: rest-api-test-run-request
tags:
- API Testing
- Java
- Load Testing
- Open Source
- Performance Testing
- Stress Testing
title: TestRunRequest
---
