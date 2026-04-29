---
description: ''
layout: schema
name: GetServiceGraphResult
properties_list:
- description: ''
  name: StartTime
  type: string
- description: ''
  name: EndTime
  type: string
- description: ''
  name: Services
  type: array
- description: ''
  name: ContainsOldGroupVersions
  type: boolean
- description: ''
  name: NextToken
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-getservicegraphresult-schema.json
slug: x-ray-getservicegraphresult
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetServiceGraphResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ReferenceId\": {\n            \"type\": \"integer\"\n          },\n          \"Name\": {\n            \"type\": \"string\"\n          },\n          \"Names\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"Root\": {\n            \"type\": \"boolean\"\n          },\n          \"AccountId\": {\n            \"type\": \"string\"\n          },\n          \"Type\": {\n            \"type\": \"string\"\n          },\n    \
  \      \"State\": {\n            \"type\": \"string\"\n          },\n          \"StartTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"EndTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"Edges\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"ReferenceId\": {\n                  \"type\": \"integer\"\n                },\n                \"StartTime\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\"\n                },\n                \"EndTime\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\"\n                },\n                \"SummaryStatistics\": {\n                  \"$ref\": \"#/components/schemas/EdgeStatistics\"\n                },\n                \"ResponseTimeHistogram\"\
  : {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"$ref\": \"#/components/schemas/HistogramEntry\"\n                  }\n                }\n              }\n            }\n          },\n          \"SummaryStatistics\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"OkCount\": {\n                \"type\": \"integer\",\n                \"format\": \"int64\"\n              },\n              \"ErrorStatistics\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"ThrottleCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  },\n                  \"OtherCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  },\n                  \"TotalCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n     \
  \             }\n                }\n              },\n              \"FaultStatistics\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"OtherCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  },\n                  \"TotalCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  }\n                }\n              },\n              \"TotalCount\": {\n                \"type\": \"integer\",\n                \"format\": \"int64\"\n              },\n              \"TotalResponseTime\": {\n                \"type\": \"number\"\n              }\n            }\n          },\n          \"ResponseTimeHistogram\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/HistogramEntry\"\n            }\n          },\n          \"DurationHistogram\": {\n            \"type\":\
  \ \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/HistogramEntry\"\n            }\n          }\n        }\n      }\n    },\n    \"ContainsOldGroupVersions\": {\n      \"type\": \"boolean\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-getservicegraphresult-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: GetServiceGraphResult
---
