---
description: Response returned immediately after a job is submitted
layout: schema
name: JobSubmitted
properties_list:
- description: Unique identifier for the submitted job
  name: jobId
  type: string
- description: URL to poll for job status
  name: statusUrl
  type: string
- description: ''
  name: _links
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-photoshop-job-submitted-schema.json
slug: adobe-creative-suite-photoshop-job-submitted
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-submitted-schema.json\",\n  \"title\": \"JobSubmitted\",\n  \"description\": \"Response returned immediately after a job is submitted\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the submitted job\",\n      \"example\": \"f54e0fcb-260b-47c3-b520-de0d17dc2b67\"\n    },\n    \"statusUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to poll for job status\",\n      \"example\": \"https://image.adobe.io/pie/psdService/status/f54e0fcb-260b-47c3-b520-de0d17dc2b67\"\n    },\n    \"_links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n \
  \             \"type\": \"string\",\n              \"example\": \"https://image.adobe.io/pie/psdService/status/f54e0fcb-260b-47c3-b520-de0d17dc2b67\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-photoshop-job-submitted-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: JobSubmitted
---
