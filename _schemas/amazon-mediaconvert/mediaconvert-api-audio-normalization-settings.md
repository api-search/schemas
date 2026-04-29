---
description: Advanced audio normalization settings. Ignore these settings unless you need to comply with a loudness standard.
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
  name: CorrectionGateLevel
  type: object
- description: ''
  name: LoudnessLogging
  type: object
- description: ''
  name: PeakCalculation
  type: object
- description: ''
  name: TargetLkfs
  type: object
- description: ''
  name: TruePeakLimiterThreshold
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-normalization-settings-schema.json
slug: mediaconvert-api-audio-normalization-settings
source_filename: mediaconvert-api-audio-normalization-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-normalization-settings-schema.json\",\n  \"title\": \"AudioNormalizationSettings\",\n  \"description\": \"Advanced audio normalization settings. Ignore these settings unless you need to comply with a loudness standard.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Algorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioNormalizationAlgorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"algorithm\"\n          },\n          \"description\": \"Choose one of the following audio normalization algorithms: ITU-R BS.1770-1: Ungated loudness. A measurement of ungated average loudness for an entire piece of content, suitable for measurement of short-form content under ATSC recommendation A/85. Supports up to 5.1\
  \ audio channels. ITU-R BS.1770-2: Gated loudness. A measurement of gated average loudness compliant with the requirements of EBU-R128. Supports up to 5.1 audio channels. ITU-R BS.1770-3: Modified peak. The same loudness measurement algorithm as 1770-2, with an updated true peak measurement. ITU-R BS.1770-4: Higher channel count. Allows for more audio channels than the other algorithms, including configurations such as 7.1.\"\n        }\n      ]\n    },\n    \"AlgorithmControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioNormalizationAlgorithmControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"algorithmControl\"\n          },\n          \"description\": \"When enabled the output audio is corrected using the chosen algorithm. If disabled, the audio will be measured but not adjusted.\"\n        }\n      ]\n    },\n    \"CorrectionGateLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative70Max0\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"correctionGateLevel\"\n          },\n          \"description\": \"Content measuring above this level will be corrected to the target level. Content measuring below this level will not be corrected.\"\n        }\n      ]\n    },\n    \"LoudnessLogging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioNormalizationLoudnessLogging\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loudnessLogging\"\n          },\n          \"description\": \"If set to LOG, log each output's audio track loudness to a CSV file.\"\n        }\n      ]\n    },\n    \"PeakCalculation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioNormalizationPeakCalculation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"peakCalculation\"\n          },\n          \"description\": \"If set to TRUE_PEAK, calculate and log the TruePeak for each\
  \ output's audio track loudness.\"\n        }\n      ]\n    },\n    \"TargetLkfs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative59Max0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetLkfs\"\n          },\n          \"description\": \"When you use Audio normalization (AudioNormalizationSettings), optionally use this setting to specify a target loudness. If you don't specify a value here, the encoder chooses a value for you, based on the algorithm that you choose for Algorithm (algorithm). If you choose algorithm 1770-1, the encoder will choose -24 LKFS; otherwise, the encoder will choose -23 LKFS.\"\n        }\n      ]\n    },\n    \"TruePeakLimiterThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMinNegative20Max0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"truePeakLimiterThreshold\"\n          },\n          \"description\": \"Specify\
  \ the True-peak limiter threshold in decibels relative to full scale (dBFS). The peak inter-audio sample loudness in your output will be limited to the value that you specify, without affecting the overall target LKFS. Enter a value from 0 to -20. Leave blank to use the default value 0.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-normalization-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioNormalizationSettings
---
