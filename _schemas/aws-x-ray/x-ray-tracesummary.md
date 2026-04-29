---
description: ''
layout: schema
name: TraceSummary
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Duration
  type: number
- description: ''
  name: ResponseTime
  type: number
- description: ''
  name: HasFault
  type: boolean
- description: ''
  name: HasError
  type: boolean
- description: ''
  name: HasThrottle
  type: boolean
- description: ''
  name: IsPartial
  type: boolean
- description: ''
  name: Http
  type: object
- description: ''
  name: Annotations
  type: object
- description: ''
  name: Users
  type: array
- description: ''
  name: ServiceIds
  type: array
- description: ''
  name: EntryPoint
  type: object
- description: ''
  name: MatchedEventTime
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-tracesummary-schema.json
slug: x-ray-tracesummary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TraceSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Duration\": {\n      \"type\": \"number\"\n    },\n    \"ResponseTime\": {\n      \"type\": \"number\"\n    },\n    \"HasFault\": {\n      \"type\": \"boolean\"\n    },\n    \"HasError\": {\n      \"type\": \"boolean\"\n    },\n    \"HasThrottle\": {\n      \"type\": \"boolean\"\n    },\n    \"IsPartial\": {\n      \"type\": \"boolean\"\n    },\n    \"Http\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"HttpURL\": {\n          \"type\": \"string\"\n        },\n        \"HttpStatus\": {\n          \"type\": \"integer\"\n        },\n        \"HttpMethod\": {\n          \"type\": \"string\"\n        },\n        \"UserAgent\": {\n          \"type\": \"string\"\n        },\n        \"ClientIp\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n\
  \    \"Annotations\": {\n      \"type\": \"object\"\n    },\n    \"Users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"UserName\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"ServiceIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\"\n          },\n          \"Names\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"AccountId\": {\n            \"type\": \"string\"\n          },\n          \"Type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"EntryPoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Name\": {\n          \"type\": \"string\"\n        },\n        \"Names\": {\n          \"type\": \"array\"\
  ,\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"AccountId\": {\n          \"type\": \"string\"\n        },\n        \"Type\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"MatchedEventTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-tracesummary-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: TraceSummary
---
