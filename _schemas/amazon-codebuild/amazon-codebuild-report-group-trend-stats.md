---
description: Contains trend statistics for a set of reports. The actual values depend on the type of trend being collected. For more information, see .
layout: schema
name: ReportGroupTrendStats
properties_list:
- description: ''
  name: average
  type: object
- description: ''
  name: max
  type: object
- description: ''
  name: min
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-report-group-trend-stats-schema.json
slug: amazon-codebuild-report-group-trend-stats
source_filename: amazon-codebuild-report-group-trend-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-group-trend-stats-schema.json\",\n  \"title\": \"ReportGroupTrendStats\",\n  \"description\": \"Contains trend statistics for a set of reports. The actual values depend on the type of trend being collected. For more information, see .\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"average\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Contains the average of all values analyzed.\"\n        }\n      ]\n    },\n    \"max\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Contains the maximum value analyzed.\"\n        }\n      ]\n    },\n    \"min\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Contains the minimum value analyzed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-group-trend-stats-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ReportGroupTrendStats
---
