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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-test-result-schema.json\",\n  \"title\": \"TestResult\",\n  \"description\": \"TestResult schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the test event was delivered successfully\"\n    },\n    \"responseCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP response code from the endpoint\"\n    },\n    \"responseTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Response time in milliseconds\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error details if the test failed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-test-result-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: TestResult
---
