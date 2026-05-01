---
description: 'Specify whether this set of input captions appears in your outputs in both 608 and 708 format. If you choose Upconvert (UPCONVERT), MediaConvert includes the captions data in two ways: it passes the 608 data through using the 608 compatibility bytes fields of the 708 wrapper, and it also translates the 608 data into 708.'
layout: schema
name: EmbeddedConvert608To708
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-embedded-convert608-to708-schema.json
slug: mediaconvert-api-embedded-convert608-to708
source_filename: mediaconvert-api-embedded-convert608-to708-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-embedded-convert608-to708-schema.json\",\n  \"title\": \"EmbeddedConvert608To708\",\n  \"description\": \"Specify whether this set of input captions appears in your outputs in both 608 and 708 format. If you choose Upconvert (UPCONVERT), MediaConvert includes the captions data in two ways: it passes the 608 data through using the 608 compatibility bytes fields of the 708 wrapper, and it also translates the 608 data into 708.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"UPCONVERT\",\n    \"DISABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-embedded-convert608-to708-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EmbeddedConvert608To708
---
