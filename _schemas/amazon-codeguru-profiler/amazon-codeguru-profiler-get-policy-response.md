---
description: The structure representing the <code>getPolicyResponse</code>.
layout: schema
name: GetPolicyResponse
properties_list:
- description: ''
  name: policy
  type: object
- description: ''
  name: revisionId
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-get-policy-response-schema.json
slug: amazon-codeguru-profiler-get-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-policy-response-schema.json\",\n  \"title\": \"GetPolicyResponse\",\n  \"description\": \"The structure representing the <code>getPolicyResponse</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The JSON-formatted resource-based policy attached to the <code>ProfilingGroup</code>.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"A unique identifier for the current revision of the returned policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policy\"\
  ,\n    \"revisionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-policy-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: GetPolicyResponse
---
