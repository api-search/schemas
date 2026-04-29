---
description: MetricDataResponse schema
layout: schema
name: MetricDataResponse
properties_list:
- description: ''
  name: metric_data
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-metric-data-response-schema.json
slug: openapi-metric-data-response
source_filename: openapi-metric-data-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-data-response-schema.json\",\n  \"title\": \"MetricDataResponse\",\n  \"description\": \"MetricDataResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric_data\": {\n      \"$ref\": \"#/components/schemas/MetricDataResponseType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-data-response-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: MetricDataResponse
---
