---
description: Response containing a list of jobs.
layout: schema
name: List Jobs Response
properties_list:
- description: ''
  name: jobs
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/list-jobs-response-schema.json
slug: list-jobs-response
source_filename: list-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/list-jobs-response-schema.json\",\n  \"title\": \"List Jobs Response\",\n  \"description\": \"Response containing a list of jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"type\": \"array\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/list-jobs-response-schema.json
tags:
- Compute
- Media
- Rendering
- Visual Effects
title: List Jobs Response
---
