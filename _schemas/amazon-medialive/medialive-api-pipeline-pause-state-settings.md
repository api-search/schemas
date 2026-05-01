---
description: Settings for pausing a pipeline.
layout: schema
name: PipelinePauseStateSettings
properties_list:
- description: ''
  name: PipelineId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-pipeline-pause-state-settings-schema.json
slug: medialive-api-pipeline-pause-state-settings
source_filename: medialive-api-pipeline-pause-state-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-pipeline-pause-state-settings-schema.json\",\n  \"title\": \"PipelinePauseStateSettings\",\n  \"description\": \"Settings for pausing a pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PipelineId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pipelineId\"\n          },\n          \"description\": \"Pipeline ID to pause (\\\"PIPELINE_0\\\" or \\\"PIPELINE_1\\\").\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PipelineId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-pipeline-pause-state-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: PipelinePauseStateSettings
---
