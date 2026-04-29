---
description: GetInsightRequest schema from Amazon X-Ray API
layout: schema
name: GetInsightRequest
properties_list:
- description: ''
  name: InsightId
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-insight-request-schema.json
slug: xray-get-insight-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"InsightId\"\n  ],\n  \"title\": \"GetInsightRequest\",\n  \"properties\": {\n    \"InsightId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightId\"\n        },\n        {\n          \"description\": \"The insight's unique identifier. Use the GetInsightSummaries action to retrieve an InsightId.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-request-schema.json\",\n  \"description\": \"GetInsightRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetInsightRequest
---
