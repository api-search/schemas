---
description: ''
layout: schema
name: Service
properties_list:
- description: ''
  name: ReferenceId
  type: integer
- description: ''
  name: Name
  type: string
- description: ''
  name: Names
  type: array
- description: ''
  name: Root
  type: boolean
- description: ''
  name: AccountId
  type: string
- description: ''
  name: Type
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: StartTime
  type: string
- description: ''
  name: EndTime
  type: string
- description: ''
  name: Edges
  type: array
- description: ''
  name: SummaryStatistics
  type: object
- description: ''
  name: ResponseTimeHistogram
  type: array
- description: ''
  name: DurationHistogram
  type: array
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-service-schema.json
slug: x-ray-service
source_filename: x-ray-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceId\": {\n      \"type\": \"integer\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Names\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"Root\": {\n      \"type\": \"boolean\"\n    },\n    \"AccountId\": {\n      \"type\": \"string\"\n    },\n    \"Type\": {\n      \"type\": \"string\"\n    },\n    \"State\": {\n      \"type\": \"string\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Edges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ReferenceId\": {\n            \"type\": \"integer\"\n          },\n          \"StartTime\"\
  : {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"EndTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"SummaryStatistics\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"OkCount\": {\n                \"type\": \"integer\",\n                \"format\": \"int64\"\n              },\n              \"ErrorStatistics\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"ThrottleCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  },\n                  \"OtherCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  },\n                  \"TotalCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  }\n           \
  \     }\n              },\n              \"FaultStatistics\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"OtherCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  },\n                  \"TotalCount\": {\n                    \"type\": \"integer\",\n                    \"format\": \"int64\"\n                  }\n                }\n              },\n              \"TotalCount\": {\n                \"type\": \"integer\",\n                \"format\": \"int64\"\n              },\n              \"TotalResponseTime\": {\n                \"type\": \"number\"\n              }\n            }\n          },\n          \"ResponseTimeHistogram\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Value\": {\n                  \"type\": \"number\"\n                },\n                \"\
  Count\": {\n                  \"type\": \"integer\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"SummaryStatistics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"OkCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"ErrorStatistics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ThrottleCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            },\n            \"OtherCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            },\n            \"TotalCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          }\n        },\n        \"FaultStatistics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"OtherCount\": {\n              \"type\": \"integer\",\n              \"format\"\
  : \"int64\"\n            },\n            \"TotalCount\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          }\n        },\n        \"TotalCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"TotalResponseTime\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"ResponseTimeHistogram\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Value\": {\n            \"type\": \"number\"\n          },\n          \"Count\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"DurationHistogram\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Value\": {\n            \"type\": \"number\"\n          },\n          \"Count\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-service-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: Service
---
