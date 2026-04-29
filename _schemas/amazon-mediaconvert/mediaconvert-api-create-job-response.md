---
description: CreateJobResponse schema from Amazon MediaConvert API
layout: schema
name: CreateJobResponse
properties_list:
- description: ''
  name: Job
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-create-job-response-schema.json
slug: mediaconvert-api-create-job-response
source_filename: mediaconvert-api-create-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-job-response-schema.json\",\n  \"title\": \"CreateJobResponse\",\n  \"description\": \"CreateJobResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Job\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Job\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"job\"\n          },\n          \"description\": \"Each job converts an input file into an output file or files. For more information, see the User Guide at https://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-job-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateJobResponse
---
