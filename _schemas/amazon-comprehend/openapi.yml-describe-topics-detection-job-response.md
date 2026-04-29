---
description: DescribeTopicsDetectionJobResponse schema
layout: schema
name: DescribeTopicsDetectionJobResponse
properties_list:
- description: ''
  name: TopicsDetectionJobProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-topics-detection-job-response-schema.json
slug: openapi.yml-describe-topics-detection-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-topics-detection-job-response-schema.json\",\n  \"title\": \"DescribeTopicsDetectionJobResponse\",\n  \"description\": \"DescribeTopicsDetectionJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TopicsDetectionJobProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicsDetectionJobProperties\"\n        },\n        {\n          \"description\": \"The list of properties for the requested job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-topics-detection-job-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeTopicsDetectionJobResponse
---
