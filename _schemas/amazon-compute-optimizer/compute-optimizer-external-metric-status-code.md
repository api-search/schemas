---
description: ExternalMetricStatusCode schema
layout: schema
name: ExternalMetricStatusCode
properties_list: []
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-external-metric-status-code-schema.json
slug: compute-optimizer-external-metric-status-code
source_filename: compute-optimizer-external-metric-status-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-external-metric-status-code-schema.json\",\n  \"title\": \"ExternalMetricStatusCode\",\n  \"description\": \"ExternalMetricStatusCode schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NO_EXTERNAL_METRIC_SET\",\n    \"INTEGRATION_SUCCESS\",\n    \"DATADOG_INTEGRATION_ERROR\",\n    \"DYNATRACE_INTEGRATION_ERROR\",\n    \"NEWRELIC_INTEGRATION_ERROR\",\n    \"INSTANA_INTEGRATION_ERROR\",\n    \"INSUFFICIENT_DATADOG_METRICS\",\n    \"INSUFFICIENT_DYNATRACE_METRICS\",\n    \"INSUFFICIENT_NEWRELIC_METRICS\",\n    \"INSUFFICIENT_INSTANA_METRICS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-external-metric-status-code-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExternalMetricStatusCode
---
