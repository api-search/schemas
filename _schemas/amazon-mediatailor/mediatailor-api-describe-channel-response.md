---
description: DescribeChannelResponse schema from Amazon MediaTailor API
layout: schema
name: DescribeChannelResponse
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
schema_file: json-schema/mediatailor-api-describe-channel-response-schema.json
slug: mediatailor-api-describe-channel-response
source_filename: mediatailor-api-describe-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-describe-channel-response-schema.json\",\n  \"title\": \"DescribeChannelResponse\",\n  \"description\": \"DescribeChannelResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The ARN of the channel.\"\n        }\n      ]\n    },\n    \"ChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the channel.\"\n        }\n      ]\n    },\n    \"ChannelState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelState\"\n        },\n        {\n          \"description\"\
  : \"Indicates whether the channel is in a running state or not.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The timestamp of when the channel was created.\"\n        }\n      ]\n    },\n    \"FillerSlate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SlateSource\"\n        },\n        {\n          \"description\": \"Contains information about the slate used to fill gaps between programs in the schedule.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The timestamp of when the channel was last modified.\"\n        }\n      ]\n    },\n    \"LogConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogConfigurationForChannel\"\
  \n        },\n        {\n          \"description\": \"The log configuration for the channel.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponseOutputs\"\n        },\n        {\n          \"description\": \"The channel's output properties.\"\n        }\n      ]\n    },\n    \"PlaybackMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The channel's playback mode.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags assigned to the channel. Tags are key-value pairs that you can associate with Amazon resources to help with organization, access control, and cost tracking. For more information, see <a\
  \ href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/tagging.html\\\">Tagging AWS Elemental MediaTailor Resources</a>.\"\n        }\n      ]\n    },\n    \"Tier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The channel's tier.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-describe-channel-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeChannelResponse
---
