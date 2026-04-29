---
description: Feedback that can be submitted for each instance of an anomaly by the user. Feedback is be used for improvements in generating recommendations for the application.
layout: schema
name: UserFeedback
properties_list:
- description: ''
  name: type
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-user-feedback-schema.json
slug: amazon-codeguru-profiler-user-feedback
source_filename: amazon-codeguru-profiler-user-feedback-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-user-feedback-schema.json\",\n  \"title\": \"UserFeedback\",\n  \"description\": \"Feedback that can be submitted for each instance of an anomaly by the user. Feedback is be used for improvements in generating recommendations for the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeedbackType\"\n        },\n        {\n          \"description\": \"Optional <code>Positive</code> or <code>Negative</code> feedback submitted by the user about whether the recommendation is useful or not.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-user-feedback-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: UserFeedback
---
