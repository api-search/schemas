---
description: TagResourceRequest schema from Amazon CodeGuru Profiler
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-tag-resource-request-schema.json
slug: amazon-codeguru-profiler-tag-resource-request
source_filename: amazon-codeguru-profiler-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon CodeGuru Profiler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \" The list of tags that are added to the specified resource. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-tag-resource-request-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: TagResourceRequest
---
