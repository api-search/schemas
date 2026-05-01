---
description: ListTopicsDetectionJobsResponse schema
layout: schema
name: ListTopicsDetectionJobsResponse
properties_list:
- description: ''
  name: TopicsDetectionJobPropertiesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-topics-detection-jobs-response-schema.json
slug: openapi.yml-list-topics-detection-jobs-response
source_filename: openapi.yml-list-topics-detection-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-topics-detection-jobs-response-schema.json\",\n  \"title\": \"ListTopicsDetectionJobsResponse\",\n  \"description\": \"ListTopicsDetectionJobsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TopicsDetectionJobPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicsDetectionJobPropertiesList\"\n        },\n        {\n          \"description\": \"A list containing the properties of each job that is returned.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-topics-detection-jobs-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListTopicsDetectionJobsResponse
---
