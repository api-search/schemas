---
description: The <code>ReadJobResponse</code> structure.
layout: schema
name: ReadJobResponse
properties_list:
- description: ''
  name: Job
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-read-job-response-schema.json
slug: amazon-elastic-transcoder-read-job-response
source_filename: amazon-elastic-transcoder-read-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-read-job-response-schema.json\",\n  \"title\": \"ReadJobResponse\",\n  \"description\": \"The <code>ReadJobResponse</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Job\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Job\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-read-job-response-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: ReadJobResponse
---
