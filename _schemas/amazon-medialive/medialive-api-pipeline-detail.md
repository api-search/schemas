---
description: Runtime details of a pipeline when a channel is running.
layout: schema
name: PipelineDetail
properties_list:
- description: ''
  name: ActiveInputAttachmentName
  type: object
- description: ''
  name: ActiveInputSwitchActionName
  type: object
- description: ''
  name: ActiveMotionGraphicsActionName
  type: object
- description: ''
  name: ActiveMotionGraphicsUri
  type: object
- description: ''
  name: PipelineId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-pipeline-detail-schema.json
slug: medialive-api-pipeline-detail
source_filename: medialive-api-pipeline-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-pipeline-detail-schema.json\",\n  \"title\": \"PipelineDetail\",\n  \"description\": \"Runtime details of a pipeline when a channel is running.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveInputAttachmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeInputAttachmentName\"\n          },\n          \"description\": \"The name of the active input attachment currently being ingested by this pipeline.\"\n        }\n      ]\n    },\n    \"ActiveInputSwitchActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeInputSwitchActionName\"\n\
  \          },\n          \"description\": \"The name of the input switch schedule action that occurred most recently and that resulted in the switch to the current input attachment for this pipeline.\"\n        }\n      ]\n    },\n    \"ActiveMotionGraphicsActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeMotionGraphicsActionName\"\n          },\n          \"description\": \"The name of the motion graphics activate action that occurred most recently and that resulted in the current graphics URI for this pipeline.\"\n        }\n      ]\n    },\n    \"ActiveMotionGraphicsUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeMotionGraphicsUri\"\n          },\n          \"description\": \"The current URI being used for HTML5 motion graphics for this\
  \ pipeline.\"\n        }\n      ]\n    },\n    \"PipelineId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pipelineId\"\n          },\n          \"description\": \"Pipeline ID\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-pipeline-detail-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: PipelineDetail
---
