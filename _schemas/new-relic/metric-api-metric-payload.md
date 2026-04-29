---
description: An array of metric data objects to be ingested
layout: schema
name: MetricPayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/metric-api-metric-payload-schema.json
slug: metric-api-metric-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-metric-payload-schema.json\",\n  \"title\": \"MetricPayload\",\n  \"description\": \"An array of metric data objects to be ingested\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/MetricDataObject\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-metric-payload-schema.json
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
title: MetricPayload
---
