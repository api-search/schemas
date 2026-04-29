---
description: The .jpg or .png file associated with an audio file.
layout: schema
name: JobAlbumArt
properties_list:
- description: ''
  name: MergePolicy
  type: object
- description: ''
  name: Artwork
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-job-album-art-schema.json
slug: amazon-elastic-transcoder-job-album-art
source_filename: amazon-elastic-transcoder-job-album-art-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-album-art-schema.json\",\n  \"title\": \"JobAlbumArt\",\n  \"description\": \"The .jpg or .png file associated with an audio file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MergePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MergePolicy\"\n        },\n        {\n          \"description\": \"<p>A policy that determines how Elastic Transcoder handles the existence of multiple album artwork files.</p> <ul> <li> <p> <code>Replace:</code> The specified album art replaces any existing album art.</p> </li> <li> <p> <code>Prepend:</code> The specified album art is placed in front of any existing album art.</p> </li> <li> <p> <code>Append:</code> The specified album art is placed after any existing album art.</p> </li>\
  \ <li> <p> <code>Fallback:</code> If the original input file contains artwork, Elastic Transcoder uses that artwork for the output. If the original input does not contain artwork, Elastic Transcoder uses the specified album art file.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Artwork\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Artworks\"\n        },\n        {\n          \"description\": \"The file to be used as album art. There can be multiple artworks associated with an audio file, to a maximum of 20. Valid formats are <code>.jpg</code> and <code>.png</code> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-album-art-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: JobAlbumArt
---
