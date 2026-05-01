---
description: Use Intra DC precision (Mpeg2IntraDcPrecision) to set quantization precision for intra-block DC coefficients. If you choose the value auto, the service will automatically select the precision based on the per-frame compression ratio.
layout: schema
name: Mpeg2IntraDcPrecision
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mpeg2-intra-dc-precision-schema.json
slug: mediaconvert-api-mpeg2-intra-dc-precision
source_filename: mediaconvert-api-mpeg2-intra-dc-precision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpeg2-intra-dc-precision-schema.json\",\n  \"title\": \"Mpeg2IntraDcPrecision\",\n  \"description\": \"Use Intra DC precision (Mpeg2IntraDcPrecision) to set quantization precision for intra-block DC coefficients. If you choose the value auto, the service will automatically select the precision based on the per-frame compression ratio.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AUTO\",\n    \"INTRA_DC_PRECISION_8\",\n    \"INTRA_DC_PRECISION_9\",\n    \"INTRA_DC_PRECISION_10\",\n    \"INTRA_DC_PRECISION_11\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpeg2-intra-dc-precision-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Mpeg2IntraDcPrecision
---
