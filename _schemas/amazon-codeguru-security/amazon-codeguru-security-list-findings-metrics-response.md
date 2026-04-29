---
description: ListFindingsMetricsResponse schema from Amazon CodeGuru Security
layout: schema
name: ListFindingsMetricsResponse
properties_list:
- description: ''
  name: findingsMetrics
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-list-findings-metrics-response-schema.json
slug: amazon-codeguru-security-list-findings-metrics-response
source_filename: amazon-codeguru-security-list-findings-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-list-findings-metrics-response-schema.json\",\n  \"title\": \"ListFindingsMetricsResponse\",\n  \"description\": \"ListFindingsMetricsResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingsMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsMetricList\"\n        },\n        {\n          \"description\": \"A list of <code>AccountFindingsMetric</code> objects retrieved from the specified time interval.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token. You can use this in future calls to <code>ListFindingMetrics</code>\
  \ to continue listing results after the current page. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-list-findings-metrics-response-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: ListFindingsMetricsResponse
---
