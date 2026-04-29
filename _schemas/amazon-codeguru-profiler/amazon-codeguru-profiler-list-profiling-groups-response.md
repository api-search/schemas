---
description: The structure representing the listProfilingGroupsResponse.
layout: schema
name: ListProfilingGroupsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: profilingGroupNames
  type: object
- description: ''
  name: profilingGroups
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-list-profiling-groups-response-schema.json
slug: amazon-codeguru-profiler-list-profiling-groups-response
source_filename: amazon-codeguru-profiler-list-profiling-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-list-profiling-groups-response-schema.json\",\n  \"title\": \"ListProfilingGroupsResponse\",\n  \"description\": \"The structure representing the listProfilingGroupsResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value to include in a future <code>ListProfilingGroups</code> request. When the results of a <code>ListProfilingGroups</code> request exceed <code>maxResults</code>, this value can be used to retrieve the next page of results. This value is <code>null</code> when there are no more results to return. \"\n        }\n      ]\n    },\n    \"profilingGroupNames\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupNames\"\n        },\n        {\n          \"description\": \" A returned list of profiling group names. A list of the names is returned only if <code>includeDescription</code> is <code>false</code>, otherwise a list of <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ProfilingGroupDescription.html\\\"> <code>ProfilingGroupDescription</code> </a> objects is returned. \"\n        }\n      ]\n    },\n    \"profilingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfilingGroupDescriptions\"\n        },\n        {\n          \"description\": \" A returned list <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ProfilingGroupDescription.html\\\"> <code>ProfilingGroupDescription</code> </a> objects. A list of <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ProfilingGroupDescription.html\\\">\
  \ <code>ProfilingGroupDescription</code> </a> objects is returned only if <code>includeDescription</code> is <code>true</code>, otherwise a list of profiling group names is returned. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profilingGroupNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-list-profiling-groups-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ListProfilingGroupsResponse
---
