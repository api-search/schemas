---
description: ListJobsResponse schema from Amazon MediaConvert API
layout: schema
name: ListJobsResponse
properties_list:
- description: ''
  name: Jobs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-list-jobs-response-schema.json
slug: mediaconvert-api-list-jobs-response
source_filename: mediaconvert-api-list-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-jobs-response-schema.json\",\n  \"title\": \"ListJobsResponse\",\n  \"description\": \"ListJobsResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfJob\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"jobs\"\n          },\n          \"description\": \"List of jobs\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Use this string to request the next batch of jobs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-jobs-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListJobsResponse
---
