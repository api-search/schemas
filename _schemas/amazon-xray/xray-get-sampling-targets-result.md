---
description: GetSamplingTargetsResult schema from Amazon X-Ray API
layout: schema
name: GetSamplingTargetsResult
properties_list:
- description: ''
  name: SamplingTargetDocuments
  type: object
- description: ''
  name: LastRuleModification
  type: object
- description: ''
  name: UnprocessedStatistics
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-sampling-targets-result-schema.json
slug: xray-get-sampling-targets-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SamplingTargetDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingTargetDocumentList\"\n        },\n        {\n          \"description\": \"Updated rules that the service should use to sample requests.\"\n        }\n      ]\n    },\n    \"LastRuleModification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time a user changed the sampling rule configuration. If the sampling rule configuration changed since the service last retrieved it, the service should call <a href=\\\"https://docs.aws.amazon.com/xray/latest/api/API_GetSamplingRules.html\\\">GetSamplingRules</a> to get the latest version.\"\n        }\n      ]\n    },\n    \"UnprocessedStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedStatisticsList\"\n        },\n \
  \       {\n          \"description\": \"Information about <a href=\\\"https://docs.aws.amazon.com/xray/latest/api/API_SamplingStatisticsDocument.html\\\">SamplingStatisticsDocument</a> that X-Ray could not process.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetSamplingTargetsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-sampling-targets-result-schema.json\",\n  \"description\": \"GetSamplingTargetsResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-sampling-targets-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetSamplingTargetsResult
---
