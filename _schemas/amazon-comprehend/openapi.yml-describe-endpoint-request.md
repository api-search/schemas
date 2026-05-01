---
description: DescribeEndpointRequest schema
layout: schema
name: DescribeEndpointRequest
properties_list:
- description: ''
  name: EndpointArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-endpoint-request-schema.json
slug: openapi.yml-describe-endpoint-request
source_filename: openapi.yml-describe-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-endpoint-request-schema.json\",\n  \"title\": \"DescribeEndpointRequest\",\n  \"description\": \"DescribeEndpointRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendEndpointArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the endpoint being described.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-endpoint-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeEndpointRequest
---
