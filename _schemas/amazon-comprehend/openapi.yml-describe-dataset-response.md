---
description: DescribeDatasetResponse schema
layout: schema
name: DescribeDatasetResponse
properties_list:
- description: ''
  name: DatasetProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-dataset-response-schema.json
slug: openapi.yml-describe-dataset-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-dataset-response-schema.json\",\n  \"title\": \"DescribeDatasetResponse\",\n  \"description\": \"DescribeDatasetResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetProperties\"\n        },\n        {\n          \"description\": \"The dataset properties.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-dataset-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeDatasetResponse
---
