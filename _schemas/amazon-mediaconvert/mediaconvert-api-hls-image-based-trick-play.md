---
description: 'Specify whether MediaConvert generates images for trick play. Keep the default value, None (NONE), to not generate any images. Choose Thumbnail (THUMBNAIL) to generate tiled thumbnails. Choose Thumbnail and full frame (THUMBNAIL_AND_FULLFRAME) to generate tiled thumbnails and full-resolution images of single frames. MediaConvert creates a child manifest for each set of images that you generate and adds corresponding entries to the parent manifest. A common application for these images is Roku trick mode. The thumbnails and full-frame images that MediaConvert creates with this feature are compatible with this Roku specification: https://developer.roku.com/docs/developer-program/media-playback/trick-mode/hls-and-dash.md'
layout: schema
name: HlsImageBasedTrickPlay
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-image-based-trick-play-schema.json
slug: mediaconvert-api-hls-image-based-trick-play
source_filename: mediaconvert-api-hls-image-based-trick-play-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-image-based-trick-play-schema.json\",\n  \"title\": \"HlsImageBasedTrickPlay\",\n  \"description\": \"Specify whether MediaConvert generates images for trick play. Keep the default value, None (NONE), to not generate any images. Choose Thumbnail (THUMBNAIL) to generate tiled thumbnails. Choose Thumbnail and full frame (THUMBNAIL_AND_FULLFRAME) to generate tiled thumbnails and full-resolution images of single frames. MediaConvert creates a child manifest for each set of images that you generate and adds corresponding entries to the parent manifest. A common application for these images is Roku trick mode. The thumbnails and full-frame images that MediaConvert creates with this feature are compatible with this Roku specification: https://developer.roku.com/docs/developer-program/media-playback/trick-mode/hls-and-dash.md\"\
  ,\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"THUMBNAIL\",\n    \"THUMBNAIL_AND_FULLFRAME\",\n    \"ADVANCED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-image-based-trick-play-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsImageBasedTrickPlay
---
