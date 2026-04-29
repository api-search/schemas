---
description: DescribeEventsDetectionJobResponse schema
layout: schema
name: DescribeEventsDetectionJobResponse
properties_list:
- description: ''
  name: EventsDetectionJobProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-events-detection-job-response-schema.json
slug: openapi.yml-describe-events-detection-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-events-detection-job-response-schema.json\",\n  \"title\": \"DescribeEventsDetectionJobResponse\",\n  \"description\": \"DescribeEventsDetectionJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventsDetectionJobProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventsDetectionJobProperties\"\n        },\n        {\n          \"description\": \"An object that contains the properties associated with an event detection job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-events-detection-job-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeEventsDetectionJobResponse
---
