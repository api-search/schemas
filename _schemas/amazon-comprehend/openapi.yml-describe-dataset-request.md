---
description: DescribeDatasetRequest schema
layout: schema
name: DescribeDatasetRequest
properties_list:
- description: ''
  name: DatasetArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-dataset-request-schema.json
slug: openapi.yml-describe-dataset-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-dataset-request-schema.json\",\n  \"title\": \"DescribeDatasetRequest\",\n  \"description\": \"DescribeDatasetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendDatasetArn\"\n        },\n        {\n          \"description\": \"The ARN of the dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatasetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-dataset-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeDatasetRequest
---
