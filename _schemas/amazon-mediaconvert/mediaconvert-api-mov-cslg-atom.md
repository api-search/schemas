---
description: When enabled, file composition times will start at zero, composition times in the 'ctts' (composition time to sample) box for B-frames will be negative, and a 'cslg' (composition shift least greatest) box will be included per 14496-1 amendment 1. This improves compatibility with Apple players and tools.
layout: schema
name: MovCslgAtom
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mov-cslg-atom-schema.json
slug: mediaconvert-api-mov-cslg-atom
source_filename: mediaconvert-api-mov-cslg-atom-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-cslg-atom-schema.json\",\n  \"title\": \"MovCslgAtom\",\n  \"description\": \"When enabled, file composition times will start at zero, composition times in the 'ctts' (composition time to sample) box for B-frames will be negative, and a 'cslg' (composition shift least greatest) box will be included per 14496-1 amendment 1. This improves compatibility with Apple players and tools.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INCLUDE\",\n    \"EXCLUDE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-cslg-atom-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MovCslgAtom
---
