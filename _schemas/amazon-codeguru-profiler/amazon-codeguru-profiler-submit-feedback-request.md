---
description: The structure representing the SubmitFeedbackRequest.
layout: schema
name: SubmitFeedbackRequest
properties_list:
- description: ''
  name: comment
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-submit-feedback-request-schema.json
slug: amazon-codeguru-profiler-submit-feedback-request
source_filename: amazon-codeguru-profiler-submit-feedback-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-submit-feedback-request-schema.json\",\n  \"title\": \"SubmitFeedbackRequest\",\n  \"description\": \"The structure representing the SubmitFeedbackRequest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Optional feedback about this anomaly.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeedbackType\"\n        },\n        {\n          \"description\": \" The feedback tpye. Thee are two valid values, <code>Positive</code> and <code>Negative</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-submit-feedback-request-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: SubmitFeedbackRequest
---
