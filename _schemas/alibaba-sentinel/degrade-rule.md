---
description: JSON Schema for Sentinel circuit breaking (degrade) rules.
layout: schema
name: Alibaba Sentinel Degrade Rule
properties_list: []
provider_name: Alibaba Sentinel
provider_slug: alibaba-sentinel
schema_file: json-schema/degrade-rule.json
slug: degrade-rule
source_filename: degrade-rule.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/alibaba-sentinel/json-schema/degrade-rule.json\",\n  \"title\": \"Alibaba Sentinel Degrade Rule\",\n  \"description\": \"JSON Schema for Sentinel circuit breaking (degrade) rules.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/$defs/DegradeRule\"\n  },\n  \"$defs\": {\n    \"DegradeRule\": {\n      \"type\": \"object\",\n      \"required\": [\"resource\", \"count\", \"grade\", \"timeWindow\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the rule.\"\n        },\n        \"resource\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name to apply the degrade rule to.\"\n        },\n        \"limitApp\": {\n          \"type\": \"string\",\n          \"default\": \"default\",\n          \"description\": \"Calling application to apply the rule\
  \ to.\"\n        },\n        \"grade\": {\n          \"type\": \"integer\",\n          \"enum\": [0, 1, 2],\n          \"description\": \"Circuit breaking strategy: 0 = slow request ratio, 1 = error ratio, 2 = error count.\"\n        },\n        \"count\": {\n          \"type\": \"number\",\n          \"description\": \"Threshold value (ratio or count depending on grade).\"\n        },\n        \"timeWindow\": {\n          \"type\": \"integer\",\n          \"description\": \"Recovery timeout in seconds.\"\n        },\n        \"minRequestAmount\": {\n          \"type\": \"integer\",\n          \"default\": 5,\n          \"description\": \"Minimum number of requests to trigger circuit breaking.\"\n        },\n        \"statIntervalMs\": {\n          \"type\": \"integer\",\n          \"default\": 1000,\n          \"description\": \"Statistics interval in milliseconds.\"\n        },\n        \"slowRatioThreshold\": {\n          \"type\": \"number\",\n          \"description\": \"Slow request\
  \ ratio threshold (for grade 0).\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alibaba-sentinel/refs/heads/main/json-schema/degrade-rule.json
tags:
- Alibaba
- Circuit Breaker
- Flow Control
- Java
- Microservices
- Rate Limiting
- Resilience
- Traffic Shaping
- Open Source
- Cloud Native
- Spring Cloud
title: Alibaba Sentinel Degrade Rule
---
