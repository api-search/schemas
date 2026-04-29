---
description: DescribeFlywheelIterationRequest schema
layout: schema
name: DescribeFlywheelIterationRequest
properties_list:
- description: ''
  name: FlywheelArn
  type: object
- description: ''
  name: FlywheelIterationId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-flywheel-iteration-request-schema.json
slug: openapi.yml-describe-flywheel-iteration-request
source_filename: openapi.yml-describe-flywheel-iteration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-flywheel-iteration-request-schema.json\",\n  \"title\": \"DescribeFlywheelIterationRequest\",\n  \"description\": \"DescribeFlywheelIterationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"FlywheelIterationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelIterationId\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlywheelArn\",\n    \"FlywheelIterationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-flywheel-iteration-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeFlywheelIterationRequest
---
