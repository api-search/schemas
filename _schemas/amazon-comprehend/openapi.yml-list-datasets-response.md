---
description: ListDatasetsResponse schema
layout: schema
name: ListDatasetsResponse
properties_list:
- description: ''
  name: DatasetPropertiesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-datasets-response-schema.json
slug: openapi.yml-list-datasets-response
source_filename: openapi.yml-list-datasets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-datasets-response-schema.json\",\n  \"title\": \"ListDatasetsResponse\",\n  \"description\": \"ListDatasetsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetPropertiesList\"\n        },\n        {\n          \"description\": \"The dataset properties list.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-datasets-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListDatasetsResponse
---
