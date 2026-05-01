---
description: DescribeSentimentDetectionJobResponse schema
layout: schema
name: DescribeSentimentDetectionJobResponse
properties_list:
- description: ''
  name: SentimentDetectionJobProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-sentiment-detection-job-response-schema.json
slug: openapi.yml-describe-sentiment-detection-job-response
source_filename: openapi.yml-describe-sentiment-detection-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-sentiment-detection-job-response-schema.json\",\n  \"title\": \"DescribeSentimentDetectionJobResponse\",\n  \"description\": \"DescribeSentimentDetectionJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SentimentDetectionJobProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SentimentDetectionJobProperties\"\n        },\n        {\n          \"description\": \"An object that contains the properties associated with a sentiment detection job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-sentiment-detection-job-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeSentimentDetectionJobResponse
---
