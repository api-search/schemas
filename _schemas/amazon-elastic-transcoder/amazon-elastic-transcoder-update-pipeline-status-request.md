---
description: The <code>UpdatePipelineStatusRequest</code> structure.
layout: schema
name: UpdatePipelineStatusRequest
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-update-pipeline-status-request-schema.json
slug: amazon-elastic-transcoder-update-pipeline-status-request
source_filename: amazon-elastic-transcoder-update-pipeline-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-status-request-schema.json\",\n  \"title\": \"UpdatePipelineStatusRequest\",\n  \"description\": \"The <code>UpdatePipelineStatusRequest</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineStatus\"\n        },\n        {\n          \"description\": \"<p>The desired status of the pipeline:</p> <ul> <li> <p> <code>Active</code>: The pipeline is processing jobs.</p> </li> <li> <p> <code>Paused</code>: The pipeline is not currently processing jobs.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-status-request-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: UpdatePipelineStatusRequest
---
