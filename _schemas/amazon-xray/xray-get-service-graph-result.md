---
description: GetServiceGraphResult schema from Amazon X-Ray API
layout: schema
name: GetServiceGraphResult
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Services
  type: object
- description: ''
  name: ContainsOldGroupVersions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-service-graph-result-schema.json
slug: xray-get-service-graph-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start of the time frame for which the graph was generated.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end of the time frame for which the graph was generated.\"\n        }\n      ]\n    },\n    \"Services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceList\"\n        },\n        {\n          \"description\": \"The services that have processed a traced request during the specified time frame.\"\n        }\n      ]\n    },\n    \"ContainsOldGroupVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"\
  description\": \"A flag indicating whether the group's filter expression has been consistent, or if the returned service graph may show traces from an older version of the group's filter expression.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetServiceGraphResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-service-graph-result-schema.json\",\n  \"description\": \"GetServiceGraphResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-service-graph-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetServiceGraphResult
---
