---
description: Audio Normalization Settings
layout: schema
name: AudioNormalizationSettings
properties_list:
- description: ''
  name: Algorithm
  type: object
- description: ''
  name: AlgorithmControl
  type: object
- description: ''
  name: TargetLkfs
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-normalization-settings-schema.json
slug: medialive-api-audio-normalization-settings
source_filename: medialive-api-audio-normalization-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-normalization-settings-schema.json\",\n  \"title\": \"AudioNormalizationSettings\",\n  \"description\": \"Audio Normalization Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Algorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioNormalizationAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"algorithm\"\n          },\n          \"description\": \"Audio normalization algorithm to use. itu17701 conforms to the CALM Act specification, itu17702 conforms to the EBU R-128 specification.\"\n        }\n      ]\n    },\n    \"AlgorithmControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioNormalizationAlgorithmControl\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"algorithmControl\"\n          },\n          \"description\": \"When set to correctAudio the output audio is corrected using the chosen algorithm. If set to measureOnly, the audio will be measured but not adjusted.\"\n        }\n      ]\n    },\n    \"TargetLkfs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative59Max0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetLkfs\"\n          },\n          \"description\": \"Target LKFS(loudness) to adjust volume to. If no value is entered, a default value will be used according to the chosen algorithm.  The CALM Act (1770-1) recommends a target of -24 LKFS. The EBU R-128 specification (1770-2) recommends a target of -23 LKFS.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-normalization-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AudioNormalizationSettings
---
