---
description: GetInsightEventsRequest schema from Amazon X-Ray API
layout: schema
name: GetInsightEventsRequest
properties_list:
- description: ''
  name: InsightId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-insight-events-request-schema.json
slug: xray-get-insight-events-request
source_filename: xray-get-insight-events-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"InsightId\"\n  ],\n  \"title\": \"GetInsightEventsRequest\",\n  \"properties\": {\n    \"InsightId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightId\"\n        },\n        {\n          \"description\": \"The insight's unique identifier. Use the GetInsightSummaries action to retrieve an InsightId.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetInsightEventsMaxResults\"\n        },\n        {\n          \"description\": \"Used to retrieve at most the specified value of events.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"Specify the pagination token returned by a previous request to retrieve the next page of events. \"\n        }\n      ]\n    }\n  },\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-events-request-schema.json\",\n  \"description\": \"GetInsightEventsRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-events-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetInsightEventsRequest
---
