---
description: GetMetricsSummaryResponse schema from Amazon CodeGuru Security
layout: schema
name: GetMetricsSummaryResponse
properties_list:
- description: ''
  name: metricsSummary
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-get-metrics-summary-response-schema.json
slug: amazon-codeguru-security-get-metrics-summary-response
source_filename: amazon-codeguru-security-get-metrics-summary-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-get-metrics-summary-response-schema.json\",\n  \"title\": \"GetMetricsSummaryResponse\",\n  \"description\": \"GetMetricsSummaryResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricsSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricsSummary\"\n        },\n        {\n          \"description\": \"The summary metrics from the specified date.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-get-metrics-summary-response-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: GetMetricsSummaryResponse
---
