---
description: Overlay motion graphics on top of your video. The motion graphics that you specify here appear on all outputs in all output groups. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/motion-graphic-overlay.html.
layout: schema
name: MotionImageInserter
properties_list:
- description: ''
  name: Framerate
  type: object
- description: ''
  name: Input
  type: object
- description: ''
  name: InsertionMode
  type: object
- description: ''
  name: Offset
  type: object
- description: ''
  name: Playback
  type: object
- description: ''
  name: StartTime
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-motion-image-inserter-schema.json
slug: mediaconvert-api-motion-image-inserter
source_filename: mediaconvert-api-motion-image-inserter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-motion-image-inserter-schema.json\",\n  \"title\": \"MotionImageInserter\",\n  \"description\": \"Overlay motion graphics on top of your video. The motion graphics that you specify here appear on all outputs in all output groups. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/motion-graphic-overlay.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Framerate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionImageInsertionFramerate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerate\"\n          },\n          \"description\": \"If your motion graphic asset is a .mov file, keep this setting unspecified. If your motion graphic asset is a series of .png files, specify the frame rate\
  \ of the overlay in frames per second, as a fraction. For example, specify 24 fps as 24/1. Make sure that the number of images in your series matches the frame rate and your intended overlay duration. For example, if you want a 30-second overlay at 30 fps, you should have 900 .png images. This overlay frame rate doesn't need to match the frame rate of the underlying video.\"\n        }\n      ]\n    },\n    \"Input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin14PatternS3Mov09PngHttpsMov09Png\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"input\"\n          },\n          \"description\": \"Specify the .mov file or series of .png files that you want to overlay on your video. For .png files, provide the file name of the first file in the series. Make sure that the names of the .png files end with sequential numbers that specify the order that they are played in. For example, overlay_000.png, overlay_001.png, overlay_002.png,\
  \ and so on. The sequence must start at zero, and each image file name must have the same number of digits. Pad your initial file names with enough zeros to complete the sequence. For example, if the first image is overlay_0.png, there can be only 10 images in the sequence, with the last image being overlay_9.png. But if the first image is overlay_00.png, there can be 100 images in the sequence.\"\n        }\n      ]\n    },\n    \"InsertionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionImageInsertionMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"insertionMode\"\n          },\n          \"description\": \"Choose the type of motion graphic asset that you are providing for your overlay. You can choose either a .mov file or a series of .png files.\"\n        }\n      ]\n    },\n    \"Offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionImageInsertionOffset\"\n        },\n    \
  \    {\n          \"xml\": {\n            \"name\": \"offset\"\n          },\n          \"description\": \"Use Offset to specify the placement of your motion graphic overlay on the video frame. Specify in pixels, from the upper-left corner of the frame. If you don't specify an offset, the service scales your overlay to the full size of the frame. Otherwise, the service inserts the overlay at its native resolution and scales the size up or down with any video scaling.\"\n        }\n      ]\n    },\n    \"Playback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionImagePlayback\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"playback\"\n          },\n          \"description\": \"Specify whether your motion graphic overlay repeats on a loop or plays only once.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin11Max11Pattern01D20305D205D\"\n   \
  \     },\n        {\n          \"xml\": {\n            \"name\": \"startTime\"\n          },\n          \"description\": \"Specify when the motion overlay begins. Use timecode format (HH:MM:SS:FF or HH:MM:SS;FF). Make sure that the timecode you provide here takes into account how you have set up your timecode configuration under both job settings and input settings. The simplest way to do that is to set both to start at 0. If you need to set up your job to follow timecodes embedded in your source that don't start at zero, make sure that you specify a start time that is after the first embedded timecode. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/setting-up-timecode.html Find job-wide and input timecode configuration settings in your JSON job settings specification at settings>timecodeConfig>source and settings>inputs>timecodeSource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-motion-image-inserter-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MotionImageInserter
---
