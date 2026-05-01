---
description: UpdateChannelRequest schema from Amazon MediaTailor API
layout: schema
name: UpdateChannelRequest
properties_list:
- description: ''
  name: FillerSlate
  type: object
- description: ''
  name: Outputs
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-update-channel-request-schema.json
slug: mediatailor-api-update-channel-request
source_filename: mediatailor-api-update-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-channel-request-schema.json\",\n  \"title\": \"UpdateChannelRequest\",\n  \"description\": \"UpdateChannelRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FillerSlate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SlateSource\"\n        },\n        {\n          \"description\": \"The slate used to fill gaps between programs in the schedule. You must configure filler slate if your channel uses the <code>LINEAR</code> <code>PlaybackMode</code>. MediaTailor doesn't support filler slate for channels using the <code>LOOP</code> <code>PlaybackMode</code>.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestOutputs\"\n    \
  \    },\n        {\n          \"description\": \"The channel's output properties.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-channel-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateChannelRequest
---
