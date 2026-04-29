---
description: DescribeEntitiesDetectionJobRequest schema
layout: schema
name: DescribeEntitiesDetectionJobRequest
properties_list:
- description: ''
  name: JobId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-entities-detection-job-request-schema.json
slug: openapi.yml-describe-entities-detection-job-request
source_filename: openapi.yml-describe-entities-detection-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entities-detection-job-request-schema.json\",\n  \"title\": \"DescribeEntitiesDetectionJobRequest\",\n  \"description\": \"DescribeEntitiesDetectionJobRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The identifier that Amazon Comprehend generated for the job. The <code>StartEntitiesDetectionJob</code> operation returns this identifier in its response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entities-detection-job-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeEntitiesDetectionJobRequest
---
