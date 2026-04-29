---
description: The properties of a Video.
layout: schema
name: VideoProperties
properties_list:
- description: Whether to enable video autoplay when the page is displayed.
  name: autoPlay
  type: boolean
- description: The time at which to start playback, measured in seconds from the beginning.
  name: start
  type: integer
- description: The time at which to end playback, measured in seconds from the beginning.
  name: end
  type: integer
- description: Whether to mute the audio during video playback.
  name: mute
  type: boolean
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-video-properties-schema.json
slug: google-slides-video-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a Video.\",\n  \"properties\": {\n    \"autoPlay\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable video autoplay when the page is displayed.\"\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"description\": \"The time at which to start playback, measured in seconds from the beginning.\"\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"description\": \"The time at which to end playback, measured in seconds from the beginning.\"\n    },\n    \"mute\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to mute the audio during video playback.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-video-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: VideoProperties
---
