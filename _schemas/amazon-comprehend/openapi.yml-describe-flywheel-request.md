---
description: DescribeFlywheelRequest schema
layout: schema
name: DescribeFlywheelRequest
properties_list:
- description: ''
  name: FlywheelArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-flywheel-request-schema.json
slug: openapi.yml-describe-flywheel-request
source_filename: openapi.yml-describe-flywheel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-flywheel-request-schema.json\",\n  \"title\": \"DescribeFlywheelRequest\",\n  \"description\": \"DescribeFlywheelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlywheelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-flywheel-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeFlywheelRequest
---
