---
description: ''
layout: schema
name: band
properties_list:
- description: cf ABPP de NITF
  name: actualBitDepth
  type: number
- description: possible values one of `RED`, `GREEN`, `BLUE`, `GRAY`, `ALPHA` or a custom string (ex `NIR`)
  name: colorInterpretation
  type: string
- description: TO BE DISCUSSED (raw, deflate,...)
  name: compression
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: isMask
  type: boolean
- description: 'The name of the **mask bands** are normalized as: - `CLD` for Cloud Cotation - `COR` for Correlation - `DET` for Detector Quality - `EXO` for Exogenous mask - `MER` for Dem merging mask - `QTE` for Te'
  name: name
  type: string
- description: the value of a pixel that does not correspond to a real data
  name: noDataValue
  type: number
- description: offset used in the buffer for this band
  name: offset
  type: number
- description: the type of pixel of the buffer
  name: pixelType
  type: string
- description: size of this band in the buffer
  name: size
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-band-schema.json
slug: oneatlas-band
source_filename: oneatlas-band-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-band-schema.json\",\n  \"title\": \"band\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actualBitDepth\": {\n      \"description\": \"cf ABPP de NITF\",\n      \"example\": 8,\n      \"format\": \"integer\",\n      \"minimum\": 0,\n      \"type\": \"number\"\n    },\n    \"colorInterpretation\": {\n      \"description\": \"possible values one of `RED`, `GREEN`, `BLUE`, `GRAY`, `ALPHA` or a custom string (ex `NIR`)\",\n      \"example\": \"GRAY\",\n      \"type\": \"string\"\n    },\n    \"compression\": {\n      \"description\": \"TO BE DISCUSSED (raw, deflate,...)\",\n      \"example\": \"raw\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"example\": \"band panchromatic\",\n      \"type\": \"string\"\n    },\n    \"isMask\": {\n      \"example\": false,\n    \
  \  \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"description\": \"The name of the **mask bands** are normalized as:\\n  - `CLD` for Cloud Cotation\\n  - `COR` for Correlation\\n  - `DET` for Detector Quality\\n  - `EXO` for Exogenous mask\\n  - `MER` for Dem merging mask\\n  - `QTE` for Technical Index\\n  - `REG` for Regulation mask\\n  - `ROI` for Area of interest\\n  - `SLT` for Saturation Cotation\\n  - `SNW` for Snow Cotation\\n  - `VAL` for Validated area mask\\n  - `VIS` for Visibility / occlusion\\n  - `VQA` for Visual control\\n  - `WAT` for Water mask\\n\\n\\nMask is a binary data always encoded in 8 bits with only 2 values:\\n  - 0 value means exclusion\\n  - 1 value means inclusion\\n\\n\\nThere is no **spectral band** name convention, it depends of the sensor. By example:\\n  - `B2`, `B1`, `B0`, `B3`, `P` for SPOT and PLEIADES\\n  - `B03`, `B01`, `B02`, `B04`, `B05`, `B06`, `B07`, `B08`, `B8A`, `B09`, `B10`, `B11`, `B12` for Sentinel2\\n  - `P` for Ref3D Ortho\\\
  n\",\n      \"example\": \"PAN\",\n      \"type\": \"string\"\n    },\n    \"noDataValue\": {\n      \"description\": \"the value of a pixel that does not correspond to a real data\",\n      \"example\": 0,\n      \"format\": \"float\",\n      \"type\": \"number\"\n    },\n    \"offset\": {\n      \"description\": \"offset used in the buffer for this band\",\n      \"example\": 0,\n      \"format\": \"integer\",\n      \"minimum\": 0,\n      \"type\": \"number\"\n    },\n    \"pixelType\": {\n      \"description\": \"the type of pixel of the buffer\",\n      \"enum\": [\n        \"Byte\",\n        \"UInt16\",\n        \"Int16\",\n        \"UInt32\",\n        \"Int32\",\n        \"Float32\",\n        \"Float64\"\n      ],\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"description\": \"size of this band in the buffer\",\n      \"example\": 25,\n      \"format\": \"integer\",\n      \"minimum\": 0,\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-band-schema.json
tags:
- Imagery
- Satellites
title: band
---
