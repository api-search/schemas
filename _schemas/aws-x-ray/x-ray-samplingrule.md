---
description: ''
layout: schema
name: SamplingRule
properties_list:
- description: ''
  name: RuleName
  type: string
- description: ''
  name: RuleARN
  type: string
- description: ''
  name: ResourceARN
  type: string
- description: ''
  name: Priority
  type: integer
- description: ''
  name: FixedRate
  type: number
- description: ''
  name: ReservoirSize
  type: integer
- description: ''
  name: ServiceName
  type: string
- description: ''
  name: ServiceType
  type: string
- description: ''
  name: Host
  type: string
- description: ''
  name: HTTPMethod
  type: string
- description: ''
  name: URLPath
  type: string
- description: ''
  name: Version
  type: integer
- description: ''
  name: Attributes
  type: object
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-samplingrule-schema.json
slug: x-ray-samplingrule
source_filename: x-ray-samplingrule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamplingRule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleName\": {\n      \"type\": \"string\"\n    },\n    \"RuleARN\": {\n      \"type\": \"string\"\n    },\n    \"ResourceARN\": {\n      \"type\": \"string\"\n    },\n    \"Priority\": {\n      \"type\": \"integer\"\n    },\n    \"FixedRate\": {\n      \"type\": \"number\"\n    },\n    \"ReservoirSize\": {\n      \"type\": \"integer\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\"\n    },\n    \"ServiceType\": {\n      \"type\": \"string\"\n    },\n    \"Host\": {\n      \"type\": \"string\"\n    },\n    \"HTTPMethod\": {\n      \"type\": \"string\"\n    },\n    \"URLPath\": {\n      \"type\": \"string\"\n    },\n    \"Version\": {\n      \"type\": \"integer\"\n    },\n    \"Attributes\": {\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"ResourceARN\",\n    \"Priority\",\n    \"FixedRate\",\n\
  \    \"ReservoirSize\",\n    \"ServiceName\",\n    \"ServiceType\",\n    \"Host\",\n    \"HTTPMethod\",\n    \"URLPath\",\n    \"Version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-samplingrule-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: SamplingRule
---
