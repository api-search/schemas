---
description: The current source for one of the pipelines in the multiplex.
layout: schema
name: MultiplexProgramPipelineDetail
properties_list:
- description: ''
  name: ActiveChannelPipeline
  type: object
- description: ''
  name: PipelineId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-program-pipeline-detail-schema.json
slug: medialive-api-multiplex-program-pipeline-detail
source_filename: medialive-api-multiplex-program-pipeline-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-pipeline-detail-schema.json\",\n  \"title\": \"MultiplexProgramPipelineDetail\",\n  \"description\": \"The current source for one of the pipelines in the multiplex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveChannelPipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeChannelPipeline\"\n          },\n          \"description\": \"Identifies the channel pipeline that is currently active for the pipeline (identified by PipelineId) in the multiplex.\"\n        }\n      ]\n    },\n    \"PipelineId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n   \
  \         \"name\": \"pipelineId\"\n          },\n          \"description\": \"Identifies a specific pipeline in the multiplex.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-pipeline-detail-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexProgramPipelineDetail
---
