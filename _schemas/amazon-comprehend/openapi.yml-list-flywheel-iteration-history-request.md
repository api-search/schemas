---
description: ListFlywheelIterationHistoryRequest schema
layout: schema
name: ListFlywheelIterationHistoryRequest
properties_list:
- description: ''
  name: FlywheelArn
  type: object
- description: ''
  name: Filter
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-flywheel-iteration-history-request-schema.json
slug: openapi.yml-list-flywheel-iteration-history-request
source_filename: openapi.yml-list-flywheel-iteration-history-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-flywheel-iteration-history-request-schema.json\",\n  \"title\": \"ListFlywheelIterationHistoryRequest\",\n  \"description\": \"ListFlywheelIterationHistoryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The ARN of the flywheel.\"\n        }\n      ]\n    },\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelIterationFilter\"\n        },\n        {\n          \"description\": \"Filter the flywheel iteration history based on creation time.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"Next token\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResultsInteger\"\n        },\n        {\n          \"description\": \"Maximum number of iteration history results to return\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlywheelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-flywheel-iteration-history-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListFlywheelIterationHistoryRequest
---
