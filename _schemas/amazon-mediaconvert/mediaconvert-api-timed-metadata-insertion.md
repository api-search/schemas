---
description: Insert user-defined custom ID3 metadata (id3) at timecodes (timecode) that you specify. In each output that you want to include this metadata, you must set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH).
layout: schema
name: TimedMetadataInsertion
properties_list:
- description: ''
  name: Id3Insertions
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-timed-metadata-insertion-schema.json
slug: mediaconvert-api-timed-metadata-insertion
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timed-metadata-insertion-schema.json\",\n  \"title\": \"TimedMetadataInsertion\",\n  \"description\": \"Insert user-defined custom ID3 metadata (id3) at timecodes (timecode) that you specify. In each output that you want to include this metadata, you must set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id3Insertions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfId3Insertion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id3Insertions\"\n          },\n          \"description\": \"Id3Insertions contains the array of Id3Insertion instances.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timed-metadata-insertion-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TimedMetadataInsertion
---
