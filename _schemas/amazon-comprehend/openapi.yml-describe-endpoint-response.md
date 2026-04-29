---
description: DescribeEndpointResponse schema
layout: schema
name: DescribeEndpointResponse
properties_list:
- description: ''
  name: EndpointProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-endpoint-response-schema.json
slug: openapi.yml-describe-endpoint-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-endpoint-response-schema.json\",\n  \"title\": \"DescribeEndpointResponse\",\n  \"description\": \"DescribeEndpointResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointProperties\"\n        },\n        {\n          \"description\": \"Describes information associated with the specific endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-endpoint-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeEndpointResponse
---
