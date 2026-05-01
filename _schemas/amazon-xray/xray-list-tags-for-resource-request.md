---
description: ListTagsForResourceRequest schema from Amazon X-Ray API
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-list-tags-for-resource-request-schema.json
slug: xray-list-tags-for-resource-request
source_filename: xray-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceARN\"\n  ],\n  \"title\": \"ListTagsForResourceRequest\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of an X-Ray group or sampling rule.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A pagination token. If multiple pages of results are returned, use the <code>NextToken</code> value returned with the current page of results as the value of this parameter to get the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-list-tags-for-resource-request-schema.json\"\
  ,\n  \"description\": \"ListTagsForResourceRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-list-tags-for-resource-request-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ListTagsForResourceRequest
---
