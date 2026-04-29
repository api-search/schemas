---
description: Filter the datasets based on creation time or dataset status.
layout: schema
name: DatasetFilter
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: DatasetType
  type: object
- description: ''
  name: CreationTimeAfter
  type: object
- description: ''
  name: CreationTimeBefore
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-filter-schema.json
slug: openapi.yml-dataset-filter
source_filename: openapi.yml-dataset-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-filter-schema.json\",\n  \"title\": \"DatasetFilter\",\n  \"description\": \"Filter the datasets based on creation time or dataset status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetStatus\"\n        },\n        {\n          \"description\": \"Filter the datasets based on the dataset status.\"\n        }\n      ]\n    },\n    \"DatasetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetType\"\n        },\n        {\n          \"description\": \"Filter the datasets based on the dataset type.\"\n        }\n      ]\n    },\n    \"CreationTimeAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n\
  \        },\n        {\n          \"description\": \"Filter the datasets to include datasets created after the specified time.\"\n        }\n      ]\n    },\n    \"CreationTimeBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filter the datasets to include datasets created before the specified time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-filter-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetFilter
---
