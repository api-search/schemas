---
description: Response indicating the metric payload was accepted for processing
layout: schema
name: IntakePayloadAccepted
properties_list:
- description: List of any non-fatal errors encountered when processing the payload
  name: errors
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-intake-payload-accepted-schema.json
slug: datadog-metrics-intake-payload-accepted
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-intake-payload-accepted-schema.json\",\n  \"title\": \"IntakePayloadAccepted\",\n  \"description\": \"Response indicating the metric payload was accepted for processing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of any non-fatal errors encountered when processing the payload\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-intake-payload-accepted-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IntakePayloadAccepted
---
