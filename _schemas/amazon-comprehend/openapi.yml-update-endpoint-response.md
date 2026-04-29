---
description: UpdateEndpointResponse schema
layout: schema
name: UpdateEndpointResponse
properties_list:
- description: ''
  name: DesiredModelArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-update-endpoint-response-schema.json
slug: openapi.yml-update-endpoint-response
source_filename: openapi.yml-update-endpoint-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-update-endpoint-response-schema.json\",\n  \"title\": \"UpdateEndpointResponse\",\n  \"description\": \"UpdateEndpointResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DesiredModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the new model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-update-endpoint-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: UpdateEndpointResponse
---
