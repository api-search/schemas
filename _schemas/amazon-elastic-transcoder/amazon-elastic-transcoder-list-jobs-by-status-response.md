---
description: The <code>ListJobsByStatusResponse</code> structure.
layout: schema
name: ListJobsByStatusResponse
properties_list:
- description: ''
  name: Jobs
  type: object
- description: ''
  name: NextPageToken
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-list-jobs-by-status-response-schema.json
slug: amazon-elastic-transcoder-list-jobs-by-status-response
source_filename: amazon-elastic-transcoder-list-jobs-by-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-list-jobs-by-status-response-schema.json\",\n  \"title\": \"ListJobsByStatusResponse\",\n  \"description\": \" The <code>ListJobsByStatusResponse</code> structure. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Jobs\"\n        },\n        {\n          \"description\": \"An array of <code>Job</code> objects that have the specified status.\"\n        }\n      ]\n    },\n    \"NextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \" A value that you use to access the second and subsequent pages of results, if any. When the jobs in the specified pipeline fit on one page or when you've\
  \ reached the last page of results, the value of <code>NextPageToken</code> is <code>null</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-list-jobs-by-status-response-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: ListJobsByStatusResponse
---
