---
description: Video Selector Pid
layout: schema
name: VideoSelectorPid
properties_list:
- description: ''
  name: Pid
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-selector-pid-schema.json
slug: medialive-api-video-selector-pid
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-pid-schema.json\",\n  \"title\": \"VideoSelectorPid\",\n  \"description\": \"Video Selector Pid\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max8191\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pid\"\n          },\n          \"description\": \"Selects a specific PID from within a video source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-pid-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoSelectorPid
---
