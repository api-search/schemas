---
description: Temporary changes to a sampling rule configuration. To meet the global sampling target for a rule, X-Ray calculates a new reservoir for each service based on the recent sampling results of all services that called <a href="https://docs.aws.amazon.com/xray/latest/api/API_GetSamplingTargets.html">GetSamplingTargets</a>.
layout: schema
name: SamplingTargetDocument
properties_list:
- description: ''
  name: RuleName
  type: object
- description: ''
  name: FixedRate
  type: object
- description: ''
  name: ReservoirQuota
  type: object
- description: ''
  name: ReservoirQuotaTTL
  type: object
- description: ''
  name: Interval
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-sampling-target-document-schema.json
slug: xray-sampling-target-document
source_filename: xray-sampling-target-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the sampling rule.\"\n        }\n      ]\n    },\n    \"FixedRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The percentage of matching requests to instrument, after the reservoir is exhausted.\"\n        }\n      ]\n    },\n    \"ReservoirQuota\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of requests per second that X-Ray allocated for this service.\"\n        }\n      ]\n    },\n    \"ReservoirQuotaTTL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"\
  When the reservoir quota expires.\"\n        }\n      ]\n    },\n    \"Interval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of seconds for the service to wait before getting sampling targets again.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Temporary changes to a sampling rule configuration. To meet the global sampling target for a rule, X-Ray calculates a new reservoir for each service based on the recent sampling results of all services that called <a href=\\\"https://docs.aws.amazon.com/xray/latest/api/API_GetSamplingTargets.html\\\">GetSamplingTargets</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamplingTargetDocument\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-target-document-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-target-document-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: SamplingTargetDocument
---
