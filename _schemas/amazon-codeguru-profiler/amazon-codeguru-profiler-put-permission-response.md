---
description: The structure representing the <code>putPermissionResponse</code>.
layout: schema
name: PutPermissionResponse
properties_list:
- description: ''
  name: policy
  type: object
- description: ''
  name: revisionId
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-put-permission-response-schema.json
slug: amazon-codeguru-profiler-put-permission-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-put-permission-response-schema.json\",\n  \"title\": \"PutPermissionResponse\",\n  \"description\": \"The structure representing the <code>putPermissionResponse</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The JSON-formatted resource-based policy on the profiling group that includes the added permissions. \"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \" A universally unique identifier (UUID) for the revision of the resource-based policy that includes the added\
  \ permissions. The JSON-formatted policy is in the <code>policy</code> element of the response. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policy\",\n    \"revisionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-put-permission-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: PutPermissionResponse
---
