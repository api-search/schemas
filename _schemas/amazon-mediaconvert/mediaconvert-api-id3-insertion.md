---
description: To insert ID3 tags in your output, specify two values. Use ID3 tag (Id3) to specify the base 64 encoded string and use Timecode (TimeCode) to specify the time when the tag should be inserted. To insert multiple ID3 tags in your output, create multiple instances of ID3 insertion (Id3Insertion).
layout: schema
name: Id3Insertion
properties_list:
- description: ''
  name: Id3
  type: object
- description: ''
  name: Timecode
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-id3-insertion-schema.json
slug: mediaconvert-api-id3-insertion
source_filename: mediaconvert-api-id3-insertion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-id3-insertion-schema.json\",\n  \"title\": \"Id3Insertion\",\n  \"description\": \"To insert ID3 tags in your output, specify two values. Use ID3 tag (Id3) to specify the base 64 encoded string and use Timecode (TimeCode) to specify the time when the tag should be inserted. To insert multiple ID3 tags in your output, create multiple instances of ID3 insertion (Id3Insertion).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternAZaZ0902\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id3\"\n          },\n          \"description\": \"Use ID3 tag (Id3) to provide a fully formed ID3 tag in base64-encode format.\"\n        }\n      ]\n    },\n    \"Timecode\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern010920405090509092\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecode\"\n          },\n          \"description\": \"Provide a Timecode (TimeCode) in HH:MM:SS:FF or HH:MM:SS;FF format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-id3-insertion-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Id3Insertion
---
