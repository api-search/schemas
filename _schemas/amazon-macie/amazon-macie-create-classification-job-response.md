---
description: CreateClassificationJobResponse schema from Amazon Macie API
layout: schema
name: CreateClassificationJobResponse
properties_list:
- description: ''
  name: jobArn
  type: object
- description: ''
  name: jobId
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-create-classification-job-response-schema.json
slug: amazon-macie-create-classification-job-response
source_filename: amazon-macie-create-classification-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-classification-job-response-schema.json\",\n  \"title\": \"CreateClassificationJobResponse\",\n  \"description\": \"CreateClassificationJobResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the job.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-classification-job-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateClassificationJobResponse
---
