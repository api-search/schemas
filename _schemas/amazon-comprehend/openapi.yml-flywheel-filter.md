---
description: Filter the flywheels based on creation time or flywheel status.
layout: schema
name: FlywheelFilter
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: CreationTimeAfter
  type: object
- description: ''
  name: CreationTimeBefore
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-flywheel-filter-schema.json
slug: openapi.yml-flywheel-filter
source_filename: openapi.yml-flywheel-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-filter-schema.json\",\n  \"title\": \"FlywheelFilter\",\n  \"description\": \"Filter the flywheels based on creation time or flywheel status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelStatus\"\n        },\n        {\n          \"description\": \"Filter the flywheels based on the flywheel status.\"\n        }\n      ]\n    },\n    \"CreationTimeAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filter the flywheels to include flywheels created after the specified time.\"\n        }\n      ]\n    },\n    \"CreationTimeBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filter the flywheels to include flywheels created before the specified time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-filter-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: FlywheelFilter
---
