---
description: Settings for ancillary captions source.
layout: schema
name: AncillarySourceSettings
properties_list:
- description: ''
  name: Convert608To708
  type: object
- description: ''
  name: SourceAncillaryChannelNumber
  type: object
- description: ''
  name: TerminateCaptions
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ancillary-source-settings-schema.json
slug: mediaconvert-api-ancillary-source-settings
source_filename: mediaconvert-api-ancillary-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ancillary-source-settings-schema.json\",\n  \"title\": \"AncillarySourceSettings\",\n  \"description\": \"Settings for ancillary captions source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Convert608To708\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AncillaryConvert608To708\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"convert608To708\"\n          },\n          \"description\": \"Specify whether this set of input captions appears in your outputs in both 608 and 708 format. If you choose Upconvert (UPCONVERT), MediaConvert includes the captions data in two ways: it passes the 608 data through using the 608 compatibility bytes fields of the 708 wrapper, and it also translates the 608 data into 708.\"\n        }\n\
  \      ]\n    },\n    \"SourceAncillaryChannelNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max4\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceAncillaryChannelNumber\"\n          },\n          \"description\": \"Specifies the 608 channel number in the ancillary data track from which to extract captions. Unused for passthrough.\"\n        }\n      ]\n    },\n    \"TerminateCaptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AncillaryTerminateCaptions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"terminateCaptions\"\n          },\n          \"description\": \"By default, the service terminates any unterminated captions at the end of each input. If you want the caption to continue onto your next input, disable this setting.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ancillary-source-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AncillarySourceSettings
---
