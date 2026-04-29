---
description: The <code>ReadPipelineResponse</code> structure.
layout: schema
name: ReadPipelineResponse
properties_list:
- description: ''
  name: Pipeline
  type: object
- description: ''
  name: Warnings
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-read-pipeline-response-schema.json
slug: amazon-elastic-transcoder-read-pipeline-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-read-pipeline-response-schema.json\",\n  \"title\": \"ReadPipelineResponse\",\n  \"description\": \"The <code>ReadPipelineResponse</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Pipeline\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the pipeline.\"\n        }\n      ]\n    },\n    \"Warnings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Warnings\"\n        },\n        {\n          \"description\": \"<p>Elastic Transcoder returns a warning if the resources used by your pipeline are not in the same region as the pipeline.</p> <p>Using resources in the\
  \ same region, such as your Amazon S3 buckets, Amazon SNS notification topics, and AWS KMS key, reduces processing time and prevents cross-regional charges.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-read-pipeline-response-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: ReadPipelineResponse
---
