---
description: A job's phase can be PROBING, TRANSCODING OR UPLOADING
layout: schema
name: JobPhase
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-job-phase-schema.json
slug: mediaconvert-api-job-phase
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-phase-schema.json\",\n  \"title\": \"JobPhase\",\n  \"description\": \"A job's phase can be PROBING, TRANSCODING OR UPLOADING\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PROBING\",\n    \"TRANSCODING\",\n    \"UPLOADING\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-phase-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: JobPhase
---
