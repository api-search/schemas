---
description: CreateDatasetGroupRequest schema from Amazon Personalize
layout: schema
name: CreateDatasetGroupRequest
properties_list:
- description: The name of the dataset group
  name: name
  type: string
- description: The domain of the dataset group
  name: domain
  type: string
provider_name: Amazon Personalize
provider_slug: amazon-personalize
schema_file: json-schema/openapi-create-dataset-group-request-schema.json
slug: openapi-create-dataset-group-request
source_filename: openapi-create-dataset-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-create-dataset-group-request-schema.json\",\n  \"title\": \"CreateDatasetGroupRequest\",\n  \"description\": \"CreateDatasetGroupRequest schema from Amazon Personalize\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dataset group\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ECOMMERCE\",\n        \"VIDEO_ON_DEMAND\"\n      ],\n      \"description\": \"The domain of the dataset group\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-create-dataset-group-request-schema.json
tags:
- AI
- Customer Experience
- Machine Learning
- ML
- Personalization
- Recommendations
title: CreateDatasetGroupRequest
---
