---
description: Information about the statistics from the code review.
layout: schema
name: Metrics
properties_list:
- description: ''
  name: MeteredLinesOfCodeCount
  type: object
- description: ''
  name: SuppressedLinesOfCodeCount
  type: object
- description: ''
  name: FindingsCount
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-metrics-schema.json
slug: amazon-codeguru-reviewer-metrics
source_filename: amazon-codeguru-reviewer-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-metrics-schema.json\",\n  \"title\": \"Metrics\",\n  \"description\": \"Information about the statistics from the code review.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MeteredLinesOfCodeCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LinesOfCodeCount\"\n        },\n        {\n          \"description\": \" <code>MeteredLinesOfCodeCount</code> is the number of lines of code in the repository where the code review happened. This does not include non-code lines such as comments and blank lines.\"\n        }\n      ]\n    },\n    \"SuppressedLinesOfCodeCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LinesOfCodeCount\"\n        },\n        {\n          \"description\": \" <code>SuppressedLinesOfCodeCount</code>\
  \ is the number of lines of code in the repository where the code review happened that CodeGuru Reviewer did not analyze. The lines suppressed in the analysis is based on the <code>excludeFiles</code> variable in the <code>aws-codeguru-reviewer.yml</code> file. This number does not include non-code lines such as comments and blank lines. \"\n        }\n      ]\n    },\n    \"FindingsCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsCount\"\n        },\n        {\n          \"description\": \"Total number of recommendations found in the code review.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-metrics-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: Metrics
---
