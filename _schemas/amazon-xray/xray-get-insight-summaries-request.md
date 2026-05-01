---
description: GetInsightSummariesRequest schema from Amazon X-Ray API
layout: schema
name: GetInsightSummariesRequest
properties_list:
- description: ''
  name: States
  type: object
- description: ''
  name: GroupARN
  type: object
- description: ''
  name: GroupName
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-insight-summaries-request-schema.json
slug: xray-get-insight-summaries-request
source_filename: xray-get-insight-summaries-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"StartTime\",\n    \"EndTime\"\n  ],\n  \"title\": \"GetInsightSummariesRequest\",\n  \"properties\": {\n    \"States\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightStateList\"\n        },\n        {\n          \"description\": \"The list of insight states. \"\n        }\n      ]\n    },\n    \"GroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the group. Required if the GroupName isn't provided.\"\n        }\n      ]\n    },\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The name of the group. Required if the GroupARN isn't provided.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The beginning of the time frame in which the insights started. The start time can't be more than 30 days old.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end of the time frame in which the insights ended. The end time can't be more than 30 days old.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetInsightSummariesMaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to display.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-summaries-request-schema.json\",\n  \"description\": \"GetInsightSummariesRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-summaries-request-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetInsightSummariesRequest
---
