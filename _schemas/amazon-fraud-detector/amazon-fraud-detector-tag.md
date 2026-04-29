---
description: A key-value metadata label applied to an Amazon Fraud Detector resource.
layout: schema
name: Tag
properties_list:
- description: Tag key.
  name: key
  type: string
- description: Tag value.
  name: value
  type: string
provider_name: Amazon Fraud Detector
provider_slug: amazon-fraud-detector
schema_file: json-schema/amazon-fraud-detector-tag-schema.json
slug: amazon-fraud-detector-tag
source_filename: amazon-fraud-detector-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value metadata label applied to an Amazon Fraud Detector resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Tag key.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Tag value.\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-tag-schema.json
tags:
- AWS
- Financial Services
- Fraud Detection
- Machine Learning
- Security
title: Tag
---
