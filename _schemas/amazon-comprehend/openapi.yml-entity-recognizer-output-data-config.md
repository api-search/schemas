---
description: Output data configuration.
layout: schema
name: EntityRecognizerOutputDataConfig
properties_list:
- description: ''
  name: FlywheelStatsS3Prefix
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognizer-output-data-config-schema.json
slug: openapi.yml-entity-recognizer-output-data-config
source_filename: openapi.yml-entity-recognizer-output-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-output-data-config-schema.json\",\n  \"title\": \"EntityRecognizerOutputDataConfig\",\n  \"description\": \"Output data configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelStatsS3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The Amazon S3 prefix for the data lake location of the flywheel statistics.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-output-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognizerOutputDataConfig
---
