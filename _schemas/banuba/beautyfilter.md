---
description: Settings for Banuba beauty filter processing.
layout: schema
name: BeautyFilter
properties_list:
- description: Skin smoothing intensity (0 = off, 1 = maximum).
  name: skinSmoothing
  type: number
- description: Face slimming intensity.
  name: faceSlimming
  type: number
- description: Eye enlarging intensity.
  name: eyeEnlarging
  type: number
- description: Teeth whitening intensity.
  name: teethWhitening
  type: number
- description: Hex color for virtual lipstick.
  name: lipstickColor
  type: string
- description: Blush effect intensity.
  name: blushIntensity
  type: number
- description: Eyebrow style preset name.
  name: eyebrowStyle
  type: string
provider_name: Banuba
provider_slug: banuba
schema_file: json-schema/beautyfilter-schema.json
slug: beautyfilter
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/banuba/json-schema/beautyfilter-schema.json\",\n  \"title\": \"BeautyFilter\",\n  \"description\": \"Settings for Banuba beauty filter processing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"skinSmoothing\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Skin smoothing intensity (0 = off, 1 = maximum).\"\n    },\n    \"faceSlimming\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Face slimming intensity.\"\n    },\n    \"eyeEnlarging\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Eye enlarging intensity.\"\n    },\n    \"teethWhitening\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Teeth whitening intensity.\"\n    },\n    \"lipstickColor\"\
  : {\n      \"type\": \"string\",\n      \"pattern\": \"^#[0-9A-Fa-f]{6}$\",\n      \"description\": \"Hex color for virtual lipstick.\"\n    },\n    \"blushIntensity\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Blush effect intensity.\"\n    },\n    \"eyebrowStyle\": {\n      \"type\": \"string\",\n      \"description\": \"Eyebrow style preset name.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/banuba/refs/heads/main/json-schema/beautyfilter-schema.json
tags:
- AR
- Augmented Reality
- Beauty
- Face Recognition
- Facial
- SDK
- Video
title: BeautyFilter
---
