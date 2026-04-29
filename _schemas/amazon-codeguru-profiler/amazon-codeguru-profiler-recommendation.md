---
description: A potential improvement that was found from analyzing the profiling data.
layout: schema
name: Recommendation
properties_list:
- description: ''
  name: allMatchesCount
  type: object
- description: ''
  name: allMatchesSum
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: pattern
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: topMatches
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-recommendation-schema.json
slug: amazon-codeguru-profiler-recommendation
source_filename: amazon-codeguru-profiler-recommendation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-recommendation-schema.json\",\n  \"title\": \"Recommendation\",\n  \"description\": \"A potential improvement that was found from analyzing the profiling data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allMatchesCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"How many different places in the profile graph triggered a match.\"\n        }\n      ]\n    },\n    \"allMatchesSum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"How much of the total sample count is potentially affected.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"End time of the profile that was used by this analysis. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC.\"\n        }\n      ]\n    },\n    \"pattern\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Pattern\"\n        },\n        {\n          \"description\": \"The pattern that analysis recognized in the profile to make this recommendation.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of the profile that was used by this analysis. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC.\"\n        }\n      ]\n    },\n\
  \    \"topMatches\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Matches\"\n        },\n        {\n          \"description\": \"List of the matches with most impact. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"allMatchesCount\",\n    \"allMatchesSum\",\n    \"endTime\",\n    \"pattern\",\n    \"startTime\",\n    \"topMatches\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-recommendation-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: Recommendation
---
