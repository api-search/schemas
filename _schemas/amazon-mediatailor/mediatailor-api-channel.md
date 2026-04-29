---
description: The configuration parameters for a channel. For information about MediaTailor channels, see <a href="https://docs.aws.amazon.com/mediatailor/latest/ug/channel-assembly-channels.html">Working with channels</a> in the <i>MediaTailor User Guide</i>.
layout: schema
name: Channel
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: ChannelName
  type: object
- description: ''
  name: ChannelState
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: FillerSlate
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: LogConfiguration
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
schema_file: json-schema/mediatailor-api-channel-schema.json
slug: mediatailor-api-channel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-channel-schema.json\",\n  \"title\": \"Channel\",\n  \"description\": \"The configuration parameters for a channel. For information about MediaTailor channels, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/channel-assembly-channels.html\\\">Working with channels</a> in the <i>MediaTailor User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The ARN of the channel.\"\n        }\n      ]\n    },\n    \"ChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the channel.\"\n        }\n      ]\n\
  \    },\n    \"ChannelState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Returns the state whether the channel is running or not.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The timestamp of when the channel was created.\"\n        }\n      ]\n    },\n    \"FillerSlate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SlateSource\"\n        },\n        {\n          \"description\": \"The slate used to fill gaps between programs in the schedule. You must configure filler slate if your channel uses the <code>LINEAR</code> <code>PlaybackMode</code>. MediaTailor doesn't support filler slate for channels using the <code>LOOP</code> <code>PlaybackMode</code>.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The timestamp of when the channel was last modified.\"\n        }\n      ]\n    },\n    \"LogConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfigurationForChannel\"\n        },\n        {\n          \"description\": \"The log configuration.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponseOutputs\"\n        },\n        {\n          \"description\": \"The channel's output properties.\"\n        }\n      ]\n    },\n    \"PlaybackMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The type of playback mode for this channel.</p> <p> <code>LINEAR</code> - Programs play back-to-back only once.</p> <p> <code>LOOP</code>\
  \ - Programs play back-to-back in an endless loop. When the last program in the schedule plays, playback loops back to the first program in the schedule.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags to assign to the channel. Tags are key-value pairs that you can associate with Amazon resources to help with organization, access control, and cost tracking. For more information, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    },\n    \"Tier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The tier for this channel. STANDARD tier channels can contain live programs.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"ChannelName\",\n    \"ChannelState\",\n    \"LogConfiguration\",\n    \"Outputs\",\n    \"PlaybackMode\",\n    \"Tier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-channel-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Channel
---
