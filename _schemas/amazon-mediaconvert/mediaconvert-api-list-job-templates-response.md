---
description: ListJobTemplatesResponse schema from Amazon MediaConvert API
layout: schema
name: ListJobTemplatesResponse
properties_list:
- description: ''
  name: JobTemplates
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-list-job-templates-response-schema.json
slug: mediaconvert-api-list-job-templates-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-job-templates-response-schema.json\",\n  \"title\": \"ListJobTemplatesResponse\",\n  \"description\": \"ListJobTemplatesResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfJobTemplate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"jobTemplates\"\n          },\n          \"description\": \"List of Job templates.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Use this string to request the next\
  \ batch of job templates.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-job-templates-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListJobTemplatesResponse
---
