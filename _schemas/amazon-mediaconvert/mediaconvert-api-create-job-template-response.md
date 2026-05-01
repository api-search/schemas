---
description: CreateJobTemplateResponse schema from Amazon MediaConvert API
layout: schema
name: CreateJobTemplateResponse
properties_list:
- description: ''
  name: JobTemplate
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-create-job-template-response-schema.json
slug: mediaconvert-api-create-job-template-response
source_filename: mediaconvert-api-create-job-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-job-template-response-schema.json\",\n  \"title\": \"CreateJobTemplateResponse\",\n  \"description\": \"CreateJobTemplateResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"jobTemplate\"\n          },\n          \"description\": \"A job template is a pre-made set of encoding instructions that you can use to quickly create a job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-job-template-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateJobTemplateResponse
---
