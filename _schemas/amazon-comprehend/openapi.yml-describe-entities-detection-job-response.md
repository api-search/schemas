---
description: DescribeEntitiesDetectionJobResponse schema
layout: schema
name: DescribeEntitiesDetectionJobResponse
properties_list:
- description: ''
  name: EntitiesDetectionJobProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-entities-detection-job-response-schema.json
slug: openapi.yml-describe-entities-detection-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entities-detection-job-response-schema.json\",\n  \"title\": \"DescribeEntitiesDetectionJobResponse\",\n  \"description\": \"DescribeEntitiesDetectionJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntitiesDetectionJobProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntitiesDetectionJobProperties\"\n        },\n        {\n          \"description\": \"An object that contains the properties associated with an entities detection job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-entities-detection-job-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeEntitiesDetectionJobResponse
---
