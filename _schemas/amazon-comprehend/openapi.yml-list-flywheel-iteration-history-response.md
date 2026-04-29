---
description: ListFlywheelIterationHistoryResponse schema
layout: schema
name: ListFlywheelIterationHistoryResponse
properties_list:
- description: ''
  name: FlywheelIterationPropertiesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-flywheel-iteration-history-response-schema.json
slug: openapi.yml-list-flywheel-iteration-history-response
source_filename: openapi.yml-list-flywheel-iteration-history-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-flywheel-iteration-history-response-schema.json\",\n  \"title\": \"ListFlywheelIterationHistoryResponse\",\n  \"description\": \"ListFlywheelIterationHistoryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelIterationPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelIterationPropertiesList\"\n        },\n        {\n          \"description\": \"List of flywheel iteration properties\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Next token\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-flywheel-iteration-history-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListFlywheelIterationHistoryResponse
---
