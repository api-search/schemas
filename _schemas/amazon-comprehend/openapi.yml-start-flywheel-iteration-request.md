---
description: StartFlywheelIterationRequest schema
layout: schema
name: StartFlywheelIterationRequest
properties_list:
- description: ''
  name: FlywheelArn
  type: object
- description: ''
  name: ClientRequestToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-start-flywheel-iteration-request-schema.json
slug: openapi.yml-start-flywheel-iteration-request
source_filename: openapi.yml-start-flywheel-iteration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-flywheel-iteration-request-schema.json\",\n  \"title\": \"StartFlywheelIterationRequest\",\n  \"description\": \"StartFlywheelIterationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The ARN of the flywheel.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"A unique identifier for the request. If you don't set the client request token, Amazon Comprehend generates one.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlywheelArn\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-flywheel-iteration-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: StartFlywheelIterationRequest
---
