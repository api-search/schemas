---
description: AggregationResponse schema from Palo Alto Networks SASE Aggregate Monitoring API
layout: schema
name: AggregationResponse
properties_list:
- description: Total number of matching records before count limit.
  name: total
  type: integer
- description: Number of records returned.
  name: count
  type: integer
- description: ''
  name: time_range
  type: object
- description: Array of result objects. Schema varies by query type and group_by dimensions.
  name: data
  type: array
- description: Time-series histogram buckets when histogram configuration was specified in the query.
  name: histogram
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-aggregate-monitoring-api-aggregation-response-schema.json
slug: sase-aggregate-monitoring-api-aggregation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AggregationResponse\",\n  \"description\": \"AggregationResponse schema from Palo Alto Networks SASE Aggregate Monitoring API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-aggregate-monitoring-api-aggregation-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching records before count limit.\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records returned.\"\n    },\n    \"time_range\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n   \
  \ \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of result objects. Schema varies by query type and group_by dimensions.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": true\n      }\n    },\n    \"histogram\": {\n      \"type\": \"array\",\n      \"description\": \"Time-series histogram buckets when histogram configuration was specified in the query.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"count\": {\n            \"type\": \"integer\"\n          },\n          \"values\": {\n            \"type\": \"object\",\n            \"additionalProperties\": true\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-aggregate-monitoring-api-aggregation-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AggregationResponse
---
