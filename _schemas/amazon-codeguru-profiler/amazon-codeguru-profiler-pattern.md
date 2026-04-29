---
description: A set of rules used to make a recommendation during an analysis.
layout: schema
name: Pattern
properties_list:
- description: ''
  name: countersToAggregate
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: resolutionSteps
  type: object
- description: ''
  name: targetFrames
  type: object
- description: ''
  name: thresholdPercent
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-pattern-schema.json
slug: amazon-codeguru-profiler-pattern
source_filename: amazon-codeguru-profiler-pattern-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-pattern-schema.json\",\n  \"title\": \"Pattern\",\n  \"description\": \" A set of rules used to make a recommendation during an analysis. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countersToAggregate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Strings\"\n        },\n        {\n          \"description\": \" A list of the different counters used to determine if there is a match. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The description of the recommendation. This explains a potential inefficiency in a profiled application.\"\n        }\n      ]\n    },\n    \"id\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The universally unique identifier (UUID) of this pattern.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name for this pattern.\"\n        }\n      ]\n    },\n    \"resolutionSteps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A string that contains the steps recommended to address the potential inefficiency. \"\n        }\n      ]\n    },\n    \"targetFrames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetFrames\"\n        },\n        {\n          \"description\": \"A list of frame names that were searched during the analysis that generated a recommendation.\"\n        }\n      ]\n \
  \   },\n    \"thresholdPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \" The percentage of time an application spends in one method that triggers a recommendation. The percentage of time is the same as the percentage of the total gathered sample counts during analysis. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-pattern-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: Pattern
---
