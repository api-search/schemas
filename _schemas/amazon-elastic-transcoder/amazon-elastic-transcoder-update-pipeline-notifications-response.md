---
description: The <code>UpdatePipelineNotificationsResponse</code> structure.
layout: schema
name: UpdatePipelineNotificationsResponse
properties_list:
- description: ''
  name: Pipeline
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-update-pipeline-notifications-response-schema.json
slug: amazon-elastic-transcoder-update-pipeline-notifications-response
source_filename: amazon-elastic-transcoder-update-pipeline-notifications-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-notifications-response-schema.json\",\n  \"title\": \"UpdatePipelineNotificationsResponse\",\n  \"description\": \"The <code>UpdatePipelineNotificationsResponse</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Pipeline\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the pipeline associated with this notification.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-notifications-response-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: UpdatePipelineNotificationsResponse
---
