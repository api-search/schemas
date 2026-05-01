---
description: Request sampling results for a single rule from a service. Results are for the last 10 seconds unless the service has been assigned a longer reporting interval after a previous call to <a href="https://docs.aws.amazon.com/xray/latest/api/API_GetSamplingTargets.html">GetSamplingTargets</a>.
layout: schema
name: SamplingStatisticsDocument
properties_list:
- description: ''
  name: RuleName
  type: object
- description: ''
  name: ClientID
  type: object
- description: ''
  name: Timestamp
  type: object
- description: ''
  name: RequestCount
  type: object
- description: ''
  name: SampledCount
  type: object
- description: ''
  name: BorrowCount
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-sampling-statistics-document-schema.json
slug: xray-sampling-statistics-document
source_filename: xray-sampling-statistics-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"RuleName\",\n    \"ClientID\",\n    \"Timestamp\",\n    \"RequestCount\",\n    \"SampledCount\"\n  ],\n  \"properties\": {\n    \"RuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleName\"\n        },\n        {\n          \"description\": \"The name of the sampling rule.\"\n        }\n      ]\n    },\n    \"ClientID\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientID\"\n        },\n        {\n          \"description\": \"A unique identifier for the service in hexadecimal.\"\n        }\n      ]\n    },\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The current time.\"\n        }\n      ]\n    },\n    \"RequestCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestCount\"\n        },\n        {\n\
  \          \"description\": \"The number of requests that matched the rule.\"\n        }\n      ]\n    },\n    \"SampledCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampledCount\"\n        },\n        {\n          \"description\": \"The number of requests recorded.\"\n        }\n      ]\n    },\n    \"BorrowCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BorrowCount\"\n        },\n        {\n          \"description\": \"The number of requests recorded with borrowed reservoir quota.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Request sampling results for a single rule from a service. Results are for the last 10 seconds unless the service has been assigned a longer reporting interval after a previous call to <a href=\\\"https://docs.aws.amazon.com/xray/latest/api/API_GetSamplingTargets.html\\\">GetSamplingTargets</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\"\
  : \"SamplingStatisticsDocument\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-statistics-document-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-statistics-document-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: SamplingStatisticsDocument
---
