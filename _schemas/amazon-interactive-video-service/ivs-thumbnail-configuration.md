---
description: An object representing a configuration of thumbnails for recorded video.
layout: schema
name: ThumbnailConfiguration
properties_list:
- description: ''
  name: recordingMode
  type: object
- description: ''
  name: resolution
  type: object
- description: ''
  name: storage
  type: object
- description: ''
  name: targetIntervalSeconds
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-thumbnail-configuration-schema.json
slug: ivs-thumbnail-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-thumbnail-configuration-schema.json\",\n  \"title\": \"ThumbnailConfiguration\",\n  \"description\": \"An object representing a configuration of thumbnails for recorded video.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recordingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingMode\"\n        },\n        {\n          \"description\": \"Thumbnail recording mode. Default: <code>INTERVAL</code>.\"\n        }\n      ]\n    },\n    \"resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThumbnailConfigurationResolution\"\n        },\n        {\n          \"description\": \"Indicates the desired resolution of recorded thumbnails. Thumbnails are recorded at the selected resolution if the corresponding\
  \ rendition is available during the stream; otherwise, they are recorded at source resolution. For more information about resolution values and their corresponding height and width dimensions, see <a href=\\\"https://docs.aws.amazon.com/ivs/latest/userguide/record-to-s3.html\\\">Auto-Record to Amazon S3</a>. Default: Null (source resolution is returned).\"\n        }\n      ]\n    },\n    \"storage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThumbnailConfigurationStorageList\"\n        },\n        {\n          \"description\": \"Indicates the format in which thumbnails are recorded. <code>SEQUENTIAL</code> records all generated thumbnails in a serial manner, to the media/thumbnails directory. <code>LATEST</code> saves the latest thumbnail in media/latest_thumbnail/thumb.jpg and overwrites it at the interval specified by <code>targetIntervalSeconds</code>. You can enable both <code>SEQUENTIAL</code> and <code>LATEST</code>. Default: <code>SEQUENTIAL</code>.\"\
  \n        }\n      ]\n    },\n    \"targetIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetIntervalSeconds\"\n        },\n        {\n          \"description\": \"<p>The targeted thumbnail-generation interval in seconds. This is configurable (and required) only if <code>recordingMode</code> is <code>INTERVAL</code>. Default: 60.</p> <p> <b>Important:</b> For the <code>BASIC</code> channel type, setting a value for <code>targetIntervalSeconds</code> does not guarantee that thumbnails are generated at the specified interval. For thumbnails to be generated at the <code>targetIntervalSeconds</code> interval, the <code>IDR/Keyframe</code> value for the input video must be less than the <code>targetIntervalSeconds</code> value. See <a href=\\\"https://docs.aws.amazon.com/ivs/latest/userguide/streaming-config.html\\\"> Amazon IVS Streaming Configuration</a> for information on setting <code>IDR/Keyframe</code> to the recommended value in video-encoder\
  \ settings.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-thumbnail-configuration-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ThumbnailConfiguration
---
