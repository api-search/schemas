---
description: GetInsightEventsResult schema from Amazon X-Ray API
layout: schema
name: GetInsightEventsResult
properties_list:
- description: ''
  name: InsightEvents
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-insight-events-result-schema.json
slug: xray-get-insight-events-result
source_filename: xray-get-insight-events-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"InsightEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightEventList\"\n        },\n        {\n          \"description\": \"A detailed description of the event. This includes the time of the event, client and root cause impact statistics, and the top anomalous service at the time of the event.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"Use this token to retrieve the next page of insight events.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetInsightEventsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-events-result-schema.json\",\n  \"description\": \"GetInsightEventsResult schema from\
  \ Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-events-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetInsightEventsResult
---
