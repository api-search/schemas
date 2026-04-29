---
description: When you update status for a pipeline, Elastic Transcoder returns the values that you specified in the request.
layout: schema
name: UpdatePipelineStatusResponse
properties_list:
- description: ''
  name: Pipeline
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-update-pipeline-status-response-schema.json
slug: amazon-elastic-transcoder-update-pipeline-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-status-response-schema.json\",\n  \"title\": \"UpdatePipelineStatusResponse\",\n  \"description\": \"When you update status for a pipeline, Elastic Transcoder returns the values that you specified in the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Pipeline\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-status-response-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: UpdatePipelineStatusResponse
---
