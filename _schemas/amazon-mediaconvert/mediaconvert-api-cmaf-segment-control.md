---
description: When set to SINGLE_FILE, a single output file is generated, which is internally segmented using the Fragment Length and Segment Length. When set to SEGMENTED_FILES, separate segment files will be created.
layout: schema
name: CmafSegmentControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-segment-control-schema.json
slug: mediaconvert-api-cmaf-segment-control
source_filename: mediaconvert-api-cmaf-segment-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-segment-control-schema.json\",\n  \"title\": \"CmafSegmentControl\",\n  \"description\": \"When set to SINGLE_FILE, a single output file is generated, which is internally segmented using the Fragment Length and Segment Length. When set to SEGMENTED_FILES, separate segment files will be created.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SINGLE_FILE\",\n    \"SEGMENTED_FILES\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-segment-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmafSegmentControl
---
