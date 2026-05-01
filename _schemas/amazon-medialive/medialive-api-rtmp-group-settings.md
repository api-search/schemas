---
description: Rtmp Group Settings
layout: schema
name: RtmpGroupSettings
properties_list:
- description: ''
  name: AdMarkers
  type: object
- description: ''
  name: AuthenticationScheme
  type: object
- description: ''
  name: CacheFullBehavior
  type: object
- description: ''
  name: CacheLength
  type: object
- description: ''
  name: CaptionData
  type: object
- description: ''
  name: InputLossAction
  type: object
- description: ''
  name: RestartDelay
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-rtmp-group-settings-schema.json
slug: medialive-api-rtmp-group-settings
source_filename: medialive-api-rtmp-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-rtmp-group-settings-schema.json\",\n  \"title\": \"RtmpGroupSettings\",\n  \"description\": \"Rtmp Group Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdMarkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfRtmpAdMarkers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adMarkers\"\n          },\n          \"description\": \"Choose the ad marker type for this output group. MediaLive will create a message based on the content of each SCTE-35 message, format it for that marker type, and insert it in the datastream.\"\n        }\n      ]\n    },\n    \"AuthenticationScheme\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationScheme\"\n        },\n        {\n          \"\
  xml\": {\n            \"name\": \"authenticationScheme\"\n          },\n          \"description\": \"Authentication scheme to use when connecting with CDN\"\n        }\n      ]\n    },\n    \"CacheFullBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RtmpCacheFullBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cacheFullBehavior\"\n          },\n          \"description\": \"Controls behavior when content cache fills up. If remote origin server stalls the RTMP connection and does not accept content fast enough the 'Media Cache' will fill up. When the cache reaches the duration specified by cacheLength the cache will stop accepting new content. If set to disconnectImmediately, the RTMP output will force a disconnect. Clear the media cache, and reconnect after restartDelay seconds. If set to waitForServer, the RTMP output will wait up to 5 minutes to allow the origin server to begin accepting data again.\"\n        }\n\
  \      ]\n    },\n    \"CacheLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin30\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cacheLength\"\n          },\n          \"description\": \"Cache length, in seconds, is used to calculate buffer size.\"\n        }\n      ]\n    },\n    \"CaptionData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RtmpCaptionData\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionData\"\n          },\n          \"description\": \"Controls the types of data that passes to onCaptionInfo outputs.  If set to 'all' then 608 and 708 carried DTVCC data will be passed.  If set to 'field1AndField2608' then DTVCC data will be stripped out, but 608 data from both fields will be passed. If set to 'field1608' then only the data carried in 608 from field 1 video will be passed.\"\n        }\n      ]\n    },\n    \"InputLossAction\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLossActionForRtmpOut\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossAction\"\n          },\n          \"description\": \"Controls the behavior of this RTMP group if input becomes unavailable.\\n\\n- emitOutput: Emit a slate until input returns.\\n- pauseOutput: Stop transmitting data until input returns. This does not close the underlying RTMP connection.\"\n        }\n      ]\n    },\n    \"RestartDelay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"restartDelay\"\n          },\n          \"description\": \"If a streaming output fails, number of seconds to wait until a restart is initiated. A value of 0 means never restart.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-rtmp-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: RtmpGroupSettings
---
