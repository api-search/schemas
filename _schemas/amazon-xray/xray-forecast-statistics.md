---
description: The predicted high and low fault count. This is used to determine if a service has become anomalous and if an insight should be created.
layout: schema
name: ForecastStatistics
properties_list:
- description: ''
  name: FaultCountHigh
  type: object
- description: ''
  name: FaultCountLow
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-forecast-statistics-schema.json
slug: xray-forecast-statistics
source_filename: xray-forecast-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FaultCountHigh\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The upper limit of fault counts for a service.\"\n        }\n      ]\n    },\n    \"FaultCountLow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The lower limit of fault counts for a service.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The predicted high and low fault count. This is used to determine if a service has become anomalous and if an insight should be created.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ForecastStatistics\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-forecast-statistics-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-forecast-statistics-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ForecastStatistics
---
