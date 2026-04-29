---
description: The structure representing the listProfileTimesResponse.
layout: schema
name: ListProfileTimesResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: profileTimes
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-list-profile-times-response-schema.json
slug: amazon-codeguru-profiler-list-profile-times-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-list-profile-times-response-schema.json\",\n  \"title\": \"ListProfileTimesResponse\",\n  \"description\": \"The structure representing the listProfileTimesResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value to include in a future <code>ListProfileTimes</code> request. When the results of a <code>ListProfileTimes</code> request exceed <code>maxResults</code>, this value can be used to retrieve the next page of results. This value is <code>null</code> when there are no more results to return. \"\n        }\n      ]\n    },\n    \"profileTimes\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/ProfileTimes\"\n        },\n        {\n          \"description\": \"The list of start times of the available profiles for the aggregation period in the specified time range. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profileTimes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-list-profile-times-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ListProfileTimesResponse
---
