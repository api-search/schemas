---
description: A job's status can be SUBMITTED, PROGRESSING, COMPLETE, CANCELED, or ERROR.
layout: schema
name: JobStatus
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-job-status-schema.json
slug: mediaconvert-api-job-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"A job's status can be SUBMITTED, PROGRESSING, COMPLETE, CANCELED, or ERROR.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SUBMITTED\",\n    \"PROGRESSING\",\n    \"COMPLETE\",\n    \"CANCELED\",\n    \"ERROR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-status-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: JobStatus
---
