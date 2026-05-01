---
description: The structure representing the <code>putPermissionRequest</code>.
layout: schema
name: PutPermissionRequest
properties_list:
- description: ''
  name: principals
  type: object
- description: ''
  name: revisionId
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-put-permission-request-schema.json
slug: amazon-codeguru-profiler-put-permission-request
source_filename: amazon-codeguru-profiler-put-permission-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-put-permission-request-schema.json\",\n  \"title\": \"PutPermissionRequest\",\n  \"description\": \"The structure representing the <code>putPermissionRequest</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"principals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Principals\"\n        },\n        {\n          \"description\": \" A list ARNs for the roles and users you want to grant access to the profiling group. Wildcards are not are supported in the ARNs. \"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \" A universally unique identifier (UUID) for the revision of the policy you\
  \ are adding to the profiling group. Do not specify this when you add permissions to a profiling group for the first time. If a policy already exists on the profiling group, you must specify the <code>revisionId</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"principals\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-put-permission-request-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: PutPermissionRequest
---
