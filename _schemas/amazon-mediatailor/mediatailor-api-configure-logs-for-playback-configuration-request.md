---
description: Configures Amazon CloudWatch log settings for a playback configuration.
layout: schema
name: ConfigureLogsForPlaybackConfigurationRequest
properties_list:
- description: ''
  name: PercentEnabled
  type: object
- description: ''
  name: PlaybackConfigurationName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-configure-logs-for-playback-configuration-request-schema.json
slug: mediatailor-api-configure-logs-for-playback-configuration-request
source_filename: mediatailor-api-configure-logs-for-playback-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-configure-logs-for-playback-configuration-request-schema.json\",\n  \"title\": \"ConfigureLogsForPlaybackConfigurationRequest\",\n  \"description\": \"Configures Amazon CloudWatch log settings for a playback configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PercentEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"<p>The percentage of session logs that MediaTailor sends to your Cloudwatch Logs account. For example, if your playback configuration has 1000 sessions and percentEnabled is set to <code>60</code>, MediaTailor sends logs for 600 of the sessions to CloudWatch Logs. MediaTailor decides at random which of the playback configuration sessions to send logs for.\
  \ If you want to view logs for a specific session, you can use the <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/debug-log-mode.html\\\">debug log mode</a>.</p> <p>Valid values: <code>0</code> - <code>100</code> </p>\"\n        }\n      ]\n    },\n    \"PlaybackConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the playback configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PercentEnabled\",\n    \"PlaybackConfigurationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-configure-logs-for-playback-configuration-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConfigureLogsForPlaybackConfigurationRequest
---
