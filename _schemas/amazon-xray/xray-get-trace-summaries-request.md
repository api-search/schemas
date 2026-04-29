---
description: GetTraceSummariesRequest schema from Amazon X-Ray API
layout: schema
name: GetTraceSummariesRequest
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: TimeRangeType
  type: object
- description: ''
  name: Sampling
  type: object
- description: ''
  name: SamplingStrategy
  type: object
- description: ''
  name: FilterExpression
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-trace-summaries-request-schema.json
slug: xray-get-trace-summaries-request
source_filename: xray-get-trace-summaries-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"StartTime\",\n    \"EndTime\"\n  ],\n  \"title\": \"GetTraceSummariesRequest\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start of the time frame for which to retrieve traces.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end of the time frame for which to retrieve traces.\"\n        }\n      ]\n    },\n    \"TimeRangeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeRangeType\"\n        },\n        {\n          \"description\": \"A parameter to indicate whether to query trace summaries by TraceId or Event time.\"\n        }\n      ]\n    },\n    \"Sampling\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Set to <code>true</code> to get summaries for only a subset of available traces.\"\n        }\n      ]\n    },\n    \"SamplingStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingStrategy\"\n        },\n        {\n          \"description\": \"A parameter to indicate whether to enable sampling on trace summaries. Input parameters are Name and Value.\"\n        }\n      ]\n    },\n    \"FilterExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterExpression\"\n        },\n        {\n          \"description\": \"Specify a filter expression to retrieve trace summaries for services or requests that meet certain requirements.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"\
  description\": \"Specify the pagination token returned by a previous request to retrieve the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-trace-summaries-request-schema.json\",\n  \"description\": \"GetTraceSummariesRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-trace-summaries-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetTraceSummariesRequest
---
