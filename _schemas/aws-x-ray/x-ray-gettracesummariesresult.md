---
description: ''
layout: schema
name: GetTraceSummariesResult
properties_list:
- description: ''
  name: TraceSummaries
  type: array
- description: ''
  name: ApproximateTime
  type: string
- description: ''
  name: TracesProcessedCount
  type: integer
- description: ''
  name: NextToken
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-gettracesummariesresult-schema.json
slug: x-ray-gettracesummariesresult
source_filename: x-ray-gettracesummariesresult-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetTraceSummariesResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TraceSummaries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Id\": {\n            \"type\": \"string\"\n          },\n          \"Duration\": {\n            \"type\": \"number\"\n          },\n          \"ResponseTime\": {\n            \"type\": \"number\"\n          },\n          \"HasFault\": {\n            \"type\": \"boolean\"\n          },\n          \"HasError\": {\n            \"type\": \"boolean\"\n          },\n          \"HasThrottle\": {\n            \"type\": \"boolean\"\n          },\n          \"IsPartial\": {\n            \"type\": \"boolean\"\n          },\n          \"Http\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"HttpURL\": {\n                \"type\": \"string\"\n        \
  \      },\n              \"HttpStatus\": {\n                \"type\": \"integer\"\n              },\n              \"HttpMethod\": {\n                \"type\": \"string\"\n              },\n              \"UserAgent\": {\n                \"type\": \"string\"\n              },\n              \"ClientIp\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"Annotations\": {\n            \"type\": \"object\"\n          },\n          \"Users\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"UserName\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"ServiceIds\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/ServiceId\"\n            }\n          },\n          \"EntryPoint\": {\n            \"type\": \"object\"\
  ,\n            \"properties\": {\n              \"Name\": {\n                \"type\": \"string\"\n              },\n              \"Names\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"AccountId\": {\n                \"type\": \"string\"\n              },\n              \"Type\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"MatchedEventTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"ApproximateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"TracesProcessedCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-gettracesummariesresult-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: GetTraceSummariesResult
---
