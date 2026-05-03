---
description: The standard JSON response envelope returned by Thanos Query API endpoints for instant and range queries. Compatible with the Prometheus API response format, with Thanos-specific additions such as partial response warnings.
layout: schema
name: Thanos Query Response
properties_list:
- description: Indicates whether the query was successful or encountered an error.
  name: status
  type: string
- description: The query result payload. Present when status is success.
  name: data
  type: object
- description: Category of error. Present when status is error.
  name: errorType
  type: string
- description: Human-readable error message. Present when status is error.
  name: error
  type: string
- description: Warnings generated during query execution. In Thanos, this often includes partial response warnings when a store is unavailable.
  name: warnings
  type: array
provider_name: Thanos
provider_slug: thanos
schema_file: json-schema/query-response.json
slug: query-response
source_filename: query-response.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://thanos.io/schemas/query-response.json\",\n  \"title\": \"Thanos Query Response\",\n  \"description\": \"The standard JSON response envelope returned by Thanos Query API endpoints for instant and range queries. Compatible with the Prometheus API response format, with Thanos-specific additions such as partial response warnings.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"status\"\n  ],\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the query was successful or encountered an error.\",\n      \"enum\": [\n        \"success\",\n        \"error\"\n      ]\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The query result payload. Present when status is success.\",\n      \"required\": [\n        \"resultType\",\n        \"result\"\n      ],\n      \"properties\": {\n        \"resultType\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The type of result returned by the query.\",\n          \"enum\": [\n            \"matrix\",\n            \"vector\",\n            \"scalar\",\n            \"string\"\n          ]\n        },\n        \"result\": {\n          \"description\": \"The query result data. Structure depends on resultType.\",\n          \"oneOf\": [\n            {\n              \"title\": \"VectorResult\",\n              \"description\": \"Result for instant vector queries.\",\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"metric\": {\n                    \"type\": \"object\",\n                    \"additionalProperties\": {\n                      \"type\": \"string\"\n                    },\n                    \"description\": \"Label set identifying the time series.\"\n                  },\n                  \"value\": {\n      \
  \              \"type\": \"array\",\n                    \"description\": \"A [unix_timestamp, sample_value] pair.\",\n                    \"prefixItems\": [\n                      {\n                        \"type\": \"number\",\n                        \"description\": \"Unix timestamp with millisecond precision.\"\n                      },\n                      {\n                        \"type\": \"string\",\n                        \"description\": \"Sample value as a string to preserve precision.\"\n                      }\n                    ],\n                    \"minItems\": 2,\n                    \"maxItems\": 2\n                  }\n                },\n                \"required\": [\n                  \"metric\",\n                  \"value\"\n                ]\n              }\n            },\n            {\n              \"title\": \"MatrixResult\",\n              \"description\": \"Result for range vector queries.\",\n              \"type\": \"array\",\n            \
  \  \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"metric\": {\n                    \"type\": \"object\",\n                    \"additionalProperties\": {\n                      \"type\": \"string\"\n                    },\n                    \"description\": \"Label set identifying the time series.\"\n                  },\n                  \"values\": {\n                    \"type\": \"array\",\n                    \"description\": \"Array of [unix_timestamp, sample_value] pairs.\",\n                    \"items\": {\n                      \"type\": \"array\",\n                      \"prefixItems\": [\n                        {\n                          \"type\": \"number\"\n                        },\n                        {\n                          \"type\": \"string\"\n                        }\n                      ],\n                      \"minItems\": 2,\n                      \"maxItems\": 2\n                 \
  \   }\n                  }\n                },\n                \"required\": [\n                  \"metric\",\n                  \"values\"\n                ]\n              }\n            },\n            {\n              \"title\": \"ScalarResult\",\n              \"description\": \"Result for scalar queries.\",\n              \"type\": \"array\",\n              \"prefixItems\": [\n                {\n                  \"type\": \"number\"\n                },\n                {\n                  \"type\": \"string\"\n                }\n              ],\n              \"minItems\": 2,\n              \"maxItems\": 2\n            },\n            {\n              \"title\": \"StringResult\",\n              \"description\": \"Result for string queries.\",\n              \"type\": \"array\",\n              \"prefixItems\": [\n                {\n                  \"type\": \"number\"\n                },\n                {\n                  \"type\": \"string\"\n                }\n        \
  \      ],\n              \"minItems\": 2,\n              \"maxItems\": 2\n            }\n          ]\n        }\n      }\n    },\n    \"errorType\": {\n      \"type\": \"string\",\n      \"description\": \"Category of error. Present when status is error.\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message. Present when status is error.\"\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"Warnings generated during query execution. In Thanos, this often includes partial response warnings when a store is unavailable.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"status\": \"success\",\n      \"data\": {\n        \"resultType\": \"vector\",\n        \"result\": [\n          {\n            \"metric\": {\n              \"__name__\": \"up\",\n              \"instance\": \"prometheus-0:9090\",\n              \"job\": \"prometheus\"\n      \
  \      },\n            \"value\": [\n              1704067200,\n              \"1\"\n            ]\n          }\n        ]\n      },\n      \"warnings\": []\n    },\n    {\n      \"status\": \"success\",\n      \"data\": {\n        \"resultType\": \"matrix\",\n        \"result\": [\n          {\n            \"metric\": {\n              \"__name__\": \"http_requests_total\",\n              \"method\": \"GET\"\n            },\n            \"values\": [\n              [1704060000, \"100\"],\n              [1704063600, \"150\"],\n              [1704067200, \"200\"]\n            ]\n          }\n        ]\n      },\n      \"warnings\": [\n        \"store sidecar-prometheus-1:10901 is unhealthy, returning partial response\"\n      ]\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/json-schema/query-response.json
tags:
- Metrics
- Monitoring
- Observability
- Prometheus
- Time Series Database
title: Thanos Query Response
---
