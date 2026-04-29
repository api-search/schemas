---
description: ConfigureLogsForChannelRequest schema from Amazon MediaTailor API
layout: schema
name: ConfigureLogsForChannelRequest
properties_list:
- description: ''
  name: ChannelName
  type: object
- description: ''
  name: LogTypes
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-configure-logs-for-channel-request-schema.json
slug: mediatailor-api-configure-logs-for-channel-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-configure-logs-for-channel-request-schema.json\",\n  \"title\": \"ConfigureLogsForChannelRequest\",\n  \"description\": \"ConfigureLogsForChannelRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the channel.\"\n        }\n      ]\n    },\n    \"LogTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogTypes\"\n        },\n        {\n          \"description\": \"The types of logs to collect.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ChannelName\",\n    \"LogTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-configure-logs-for-channel-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConfigureLogsForChannelRequest
---
