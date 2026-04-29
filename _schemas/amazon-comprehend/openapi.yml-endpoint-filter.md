---
description: The filter used to determine which endpoints are returned. You can filter jobs on their name, model, status, or the date and time that they were created. You can only set one filter at a time.
layout: schema
name: EndpointFilter
properties_list:
- description: ''
  name: ModelArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreationTimeBefore
  type: object
- description: ''
  name: CreationTimeAfter
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-endpoint-filter-schema.json
slug: openapi.yml-endpoint-filter
source_filename: openapi.yml-endpoint-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-endpoint-filter-schema.json\",\n  \"title\": \"EndpointFilter\",\n  \"description\": \"The filter used to determine which endpoints are returned. You can filter jobs on their name, model, status, or the date and time that they were created. You can only set one filter at a time. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the model to which the endpoint is attached.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointStatus\"\n        },\n        {\n          \"description\": \"Specifies the status of\
  \ the endpoint being returned. Possible values are: Creating, Ready, Updating, Deleting, Failed.\"\n        }\n      ]\n    },\n    \"CreationTimeBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Specifies a date before which the returned endpoint or endpoints were created.\"\n        }\n      ]\n    },\n    \"CreationTimeAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Specifies a date after which the returned endpoint or endpoints were created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-endpoint-filter-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EndpointFilter
---
