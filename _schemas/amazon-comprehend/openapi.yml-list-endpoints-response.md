---
description: ListEndpointsResponse schema
layout: schema
name: ListEndpointsResponse
properties_list:
- description: ''
  name: EndpointPropertiesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-endpoints-response-schema.json
slug: openapi.yml-list-endpoints-response
source_filename: openapi.yml-list-endpoints-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-endpoints-response-schema.json\",\n  \"title\": \"ListEndpointsResponse\",\n  \"description\": \"ListEndpointsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointPropertiesList\"\n        },\n        {\n          \"description\": \"Displays a list of endpoint properties being retrieved by the service in response to the request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-endpoints-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListEndpointsResponse
---
