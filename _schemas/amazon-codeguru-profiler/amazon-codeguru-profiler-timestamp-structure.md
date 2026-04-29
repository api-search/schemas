---
description: A data type that contains a <code>Timestamp</code> object. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC.
layout: schema
name: TimestampStructure
properties_list:
- description: ''
  name: value
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-timestamp-structure-schema.json
slug: amazon-codeguru-profiler-timestamp-structure
source_filename: amazon-codeguru-profiler-timestamp-structure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-timestamp-structure-schema.json\",\n  \"title\": \"TimestampStructure\",\n  \"description\": \" A data type that contains a <code>Timestamp</code> object. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" A <code>Timestamp</code>. This is specified using the ISO 8601 format. For example, 2020-06-01T13:15:02.001Z represents 1 millisecond past June 1, 2020 1:15:02 PM UTC. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-timestamp-structure-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: TimestampStructure
---
