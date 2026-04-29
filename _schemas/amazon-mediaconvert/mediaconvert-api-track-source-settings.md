---
description: Settings specific to caption sources that are specified by track number. Currently, this is only IMSC captions in an IMF package. If your caption source is IMSC 1.1 in a separate xml file, use FileSourceSettings instead of TrackSourceSettings.
layout: schema
name: TrackSourceSettings
properties_list:
- description: ''
  name: TrackNumber
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-track-source-settings-schema.json
slug: mediaconvert-api-track-source-settings
source_filename: mediaconvert-api-track-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-track-source-settings-schema.json\",\n  \"title\": \"TrackSourceSettings\",\n  \"description\": \"Settings specific to caption sources that are specified by track number. Currently, this is only IMSC captions in an IMF package. If your caption source is IMSC 1.1 in a separate xml file, use FileSourceSettings instead of TrackSourceSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TrackNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"trackNumber\"\n          },\n          \"description\": \"Use this setting to select a single captions track from a source. Track numbers correspond to the order in the captions source file. For IMF sources,\
  \ track numbering is based on the order that the captions appear in the CPL. For example, use 1 to select the captions asset that is listed first in the CPL. To include more than one captions track in your job outputs, create multiple input captions selectors. Specify one track per selector.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-track-source-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TrackSourceSettings
---
