---
description: ''
layout: schema
name: SamplingRuleRecord
properties_list:
- description: ''
  name: SamplingRule
  type: object
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: ModifiedAt
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-samplingrulerecord-schema.json
slug: x-ray-samplingrulerecord
source_filename: x-ray-samplingrulerecord-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamplingRuleRecord\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SamplingRule\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"RuleName\": {\n          \"type\": \"string\"\n        },\n        \"RuleARN\": {\n          \"type\": \"string\"\n        },\n        \"ResourceARN\": {\n          \"type\": \"string\"\n        },\n        \"Priority\": {\n          \"type\": \"integer\"\n        },\n        \"FixedRate\": {\n          \"type\": \"number\"\n        },\n        \"ReservoirSize\": {\n          \"type\": \"integer\"\n        },\n        \"ServiceName\": {\n          \"type\": \"string\"\n        },\n        \"ServiceType\": {\n          \"type\": \"string\"\n        },\n        \"Host\": {\n          \"type\": \"string\"\n        },\n        \"HTTPMethod\": {\n          \"type\": \"string\"\n        },\n        \"URLPath\": {\n          \"type\": \"string\"\
  \n        },\n        \"Version\": {\n          \"type\": \"integer\"\n        },\n        \"Attributes\": {\n          \"type\": \"object\"\n        }\n      },\n      \"required\": [\n        \"ResourceARN\",\n        \"Priority\",\n        \"FixedRate\",\n        \"ReservoirSize\",\n        \"ServiceName\",\n        \"ServiceType\",\n        \"Host\",\n        \"HTTPMethod\",\n        \"URLPath\",\n        \"Version\"\n      ]\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"ModifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-samplingrulerecord-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: SamplingRuleRecord
---
