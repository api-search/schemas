---
description: ConfigureLogsForPlaybackConfigurationResponse schema from Amazon MediaTailor API
layout: schema
name: ConfigureLogsForPlaybackConfigurationResponse
properties_list:
- description: ''
  name: PercentEnabled
  type: object
- description: ''
  name: PlaybackConfigurationName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-configure-logs-for-playback-configuration-response-schema.json
slug: mediatailor-api-configure-logs-for-playback-configuration-response
source_filename: mediatailor-api-configure-logs-for-playback-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-configure-logs-for-playback-configuration-response-schema.json\",\n  \"title\": \"ConfigureLogsForPlaybackConfigurationResponse\",\n  \"description\": \"ConfigureLogsForPlaybackConfigurationResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PercentEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The percentage of session logs that MediaTailor sends to your Cloudwatch Logs account.\"\n        }\n      ]\n    },\n    \"PlaybackConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the playback configuration.\"\n      \
  \  }\n      ]\n    }\n  },\n  \"required\": [\n    \"PercentEnabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-configure-logs-for-playback-configuration-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ConfigureLogsForPlaybackConfigurationResponse
---
