---
description: DescribeFlywheelResponse schema
layout: schema
name: DescribeFlywheelResponse
properties_list:
- description: ''
  name: FlywheelProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-flywheel-response-schema.json
slug: openapi.yml-describe-flywheel-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-flywheel-response-schema.json\",\n  \"title\": \"DescribeFlywheelResponse\",\n  \"description\": \"DescribeFlywheelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelProperties\"\n        },\n        {\n          \"description\": \"The flywheel properties.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-flywheel-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeFlywheelResponse
---
