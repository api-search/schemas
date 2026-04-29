---
description: Describes the information about an entity recognizer and its versions.
layout: schema
name: EntityRecognizerSummary
properties_list:
- description: ''
  name: RecognizerName
  type: object
- description: ''
  name: NumberOfVersions
  type: object
- description: ''
  name: LatestVersionCreatedAt
  type: object
- description: ''
  name: LatestVersionName
  type: object
- description: ''
  name: LatestVersionStatus
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognizer-summary-schema.json
slug: openapi.yml-entity-recognizer-summary
source_filename: openapi.yml-entity-recognizer-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-summary-schema.json\",\n  \"title\": \"EntityRecognizerSummary\",\n  \"description\": \" Describes the information about an entity recognizer and its versions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecognizerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \" The name that you assigned the entity recognizer.\"\n        }\n      ]\n    },\n    \"NumberOfVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of versions you created.\"\n        }\n      ]\n    },\n    \"LatestVersionCreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The time that the latest entity recognizer version was submitted for processing.\"\n        }\n      ]\n    },\n    \"LatestVersionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionName\"\n        },\n        {\n          \"description\": \" The version name you assigned to the latest entity recognizer version.\"\n        }\n      ]\n    },\n    \"LatestVersionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatus\"\n        },\n        {\n          \"description\": \" Provides the status of the latest entity recognizer version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-summary-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognizerSummary
---
