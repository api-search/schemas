---
description: Indicates which pipeline is preferred by the multiplex for program ingest. If set to \"PIPELINE_0\" or \"PIPELINE_1\" and an unhealthy ingest causes the multiplex to switch to the non-preferred pipeline, it will switch back once that ingest is healthy again. If set to \"CURRENTLY_ACTIVE\", it will not switch back to the other pipeline based on it recovering to a healthy state, it will only switch if the active pipeline becomes unhealthy.
layout: schema
name: PreferredChannelPipeline
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-preferred-channel-pipeline-schema.json
slug: medialive-api-preferred-channel-pipeline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-preferred-channel-pipeline-schema.json\",\n  \"title\": \"PreferredChannelPipeline\",\n  \"description\": \"Indicates which pipeline is preferred by the multiplex for program ingest.\\nIf set to \\\\\\\"PIPELINE_0\\\\\\\" or \\\\\\\"PIPELINE_1\\\\\\\" and an unhealthy ingest causes the multiplex to switch to the non-preferred pipeline,\\nit will switch back once that ingest is healthy again. If set to \\\\\\\"CURRENTLY_ACTIVE\\\\\\\",\\nit will not switch back to the other pipeline based on it recovering to a healthy state,\\nit will only switch if the active pipeline becomes unhealthy.\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CURRENTLY_ACTIVE\",\n    \"PIPELINE_0\",\n    \"PIPELINE_1\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-preferred-channel-pipeline-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PreferredChannelPipeline
---
