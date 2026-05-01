---
description: Provides information for filtering a list of entity recognizers. You can only specify one filtering parameter in a request. For more information, see the <code>ListEntityRecognizers</code> operation./&gt;
layout: schema
name: EntityRecognizerFilter
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: RecognizerName
  type: object
- description: ''
  name: SubmitTimeBefore
  type: object
- description: ''
  name: SubmitTimeAfter
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognizer-filter-schema.json
slug: openapi.yml-entity-recognizer-filter
source_filename: openapi.yml-entity-recognizer-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-filter-schema.json\",\n  \"title\": \"EntityRecognizerFilter\",\n  \"description\": \"Provides information for filtering a list of entity recognizers. You can only specify one filtering parameter in a request. For more information, see the <code>ListEntityRecognizers</code> operation./&gt;\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatus\"\n        },\n        {\n          \"description\": \"The status of an entity recognizer.\"\n        }\n      ]\n    },\n    \"RecognizerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"The name that you assigned the entity recognizer.\"\
  \n        }\n      ]\n    },\n    \"SubmitTimeBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filters the list of entities based on the time that the list was submitted for processing. Returns only jobs submitted before the specified time. Jobs are returned in descending order, newest to oldest.\"\n        }\n      ]\n    },\n    \"SubmitTimeAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filters the list of entities based on the time that the list was submitted for processing. Returns only jobs submitted after the specified time. Jobs are returned in ascending order, oldest to newest.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-filter-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognizerFilter
---
