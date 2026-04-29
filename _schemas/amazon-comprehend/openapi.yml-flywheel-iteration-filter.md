---
description: Filter the flywheel iterations based on creation time.
layout: schema
name: FlywheelIterationFilter
properties_list:
- description: ''
  name: CreationTimeAfter
  type: object
- description: ''
  name: CreationTimeBefore
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-flywheel-iteration-filter-schema.json
slug: openapi.yml-flywheel-iteration-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-iteration-filter-schema.json\",\n  \"title\": \"FlywheelIterationFilter\",\n  \"description\": \"Filter the flywheel iterations based on creation time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreationTimeAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filter the flywheel iterations to include iterations created after the specified time.\"\n        }\n      ]\n    },\n    \"CreationTimeBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filter the flywheel iterations to include iterations created before the specified time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-iteration-filter-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: FlywheelIterationFilter
---
