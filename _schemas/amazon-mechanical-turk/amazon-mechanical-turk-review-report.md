---
description: Contains both ReviewResult and ReviewAction elements for a particular HIT.
layout: schema
name: ReviewReport
properties_list:
- description: ''
  name: ReviewResults
  type: object
- description: ''
  name: ReviewActions
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-review-report-schema.json
slug: amazon-mechanical-turk-review-report
source_filename: amazon-mechanical-turk-review-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-report-schema.json\",\n  \"title\": \"ReviewReport\",\n  \"description\": \" Contains both ReviewResult and ReviewAction elements for a particular HIT. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReviewResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewResultDetailList\"\n        },\n        {\n          \"description\": \" A list of ReviewResults objects for each action specified in the Review Policy. \"\n        }\n      ]\n    },\n    \"ReviewActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewActionDetailList\"\n        },\n        {\n          \"description\": \" A list of ReviewAction objects for each action specified in the Review Policy. \"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-report-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ReviewReport
---
