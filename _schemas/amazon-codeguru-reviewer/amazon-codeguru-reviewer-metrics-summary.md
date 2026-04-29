---
description: Information about metrics summaries.
layout: schema
name: MetricsSummary
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
schema_file: json-schema/amazon-codeguru-reviewer-metrics-summary-schema.json
slug: amazon-codeguru-reviewer-metrics-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-metrics-summary-schema.json\",\n  \"title\": \"MetricsSummary\",\n  \"description\": \"Information about metrics summaries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MeteredLinesOfCodeCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LinesOfCodeCount\"\n        },\n        {\n          \"description\": \"Lines of code metered in the code review. For the initial code review pull request and all subsequent revisions, this includes all lines of code in the files added to the pull request. In subsequent revisions, for files that already existed in the pull request, this includes only the changed lines of code. In both cases, this does not include non-code lines such as comments and import statements. For example, if you submit\
  \ a pull request containing 5 files, each with 500 lines of code, and in a subsequent revision you added a new file with 200 lines of code, and also modified a total of 25 lines across the initial 5 files, <code>MeteredLinesOfCodeCount</code> includes the first 5 files (5 * 500 = 2,500 lines), the new file (200 lines) and the 25 changed lines of code for a total of 2,725 lines of code.\"\n        }\n      ]\n    },\n    \"SuppressedLinesOfCodeCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LinesOfCodeCount\"\n        },\n        {\n          \"description\": \"Lines of code suppressed in the code review based on the <code>excludeFiles</code> element in the <code>aws-codeguru-reviewer.yml</code> file. For full repository analyses, this number includes all lines of code in the files that are suppressed. For pull requests, this number only includes the <i>changed</i> lines of code that are suppressed. In both cases, this number does not include non-code\
  \ lines such as comments and import statements. For example, if you initiate a full repository analysis on a repository containing 5 files, each file with 100 lines of code, and 2 files are listed as excluded in the <code>aws-codeguru-reviewer.yml</code> file, then <code>SuppressedLinesOfCodeCount</code> returns 200 (2 * 100) as the total number of lines of code suppressed. However, if you submit a pull request for the same repository, then <code>SuppressedLinesOfCodeCount</code> only includes the lines in the 2 files that changed. If only 1 of the 2 files changed in the pull request, then <code>SuppressedLinesOfCodeCount</code> returns 100 (1 * 100) as the total number of lines of code suppressed.\"\n        }\n      ]\n    },\n    \"FindingsCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsCount\"\n        },\n        {\n          \"description\": \"Total number of recommendations found in the code review.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-metrics-summary-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: MetricsSummary
---
