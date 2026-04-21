---
description: TestResult schema from ARGUS Enterprise API
layout: schema
name: TestResult
properties_list:
- description: Whether the test event was delivered successfully
  name: success
  type: boolean
- description: HTTP response code from the endpoint
  name: responseCode
  type: integer
- description: Response time in milliseconds
  name: responseTime
  type: integer
- description: Error details if the test failed
  name: errorMessage
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-test-result-schema.json
slug: argus-enterprise-test-result
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: TestResult
---
