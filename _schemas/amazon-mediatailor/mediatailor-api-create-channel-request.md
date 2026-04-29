---
description: CreateChannelRequest schema from Amazon MediaTailor API
layout: schema
name: CreateChannelRequest
properties_list:
- description: ''
  name: FillerSlate
  type: object
- description: ''
  name: Outputs
  type: object
- description: ''
  name: PlaybackMode
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Tier
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-channel-request-schema.json
slug: mediatailor-api-create-channel-request
source_filename: mediatailor-api-create-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-channel-request-schema.json\",\n  \"title\": \"CreateChannelRequest\",\n  \"description\": \"CreateChannelRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FillerSlate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SlateSource\"\n        },\n        {\n          \"description\": \"The slate used to fill gaps between programs in the schedule. You must configure filler slate if your channel uses the <code>LINEAR</code> <code>PlaybackMode</code>. MediaTailor doesn't support filler slate for channels using the <code>LOOP</code> <code>PlaybackMode</code>.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestOutputs\"\n    \
  \    },\n        {\n          \"description\": \"The channel's output properties.\"\n        }\n      ]\n    },\n    \"PlaybackMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackMode\"\n        },\n        {\n          \"description\": \"<p>The type of playback mode to use for this channel.</p> <p> <code>LINEAR</code> - The programs in the schedule play once back-to-back in the schedule.</p> <p> <code>LOOP</code> - The programs in the schedule play back-to-back in an endless loop. When the last program in the schedule stops playing, playback loops back to the first program in the schedule.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags to assign to the channel. Tags are key-value pairs that you can associate with Amazon resources\
  \ to help with organization, access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    },\n    \"Tier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tier\"\n        },\n        {\n          \"description\": \"The tier of the channel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Outputs\",\n    \"PlaybackMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-channel-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateChannelRequest
---
