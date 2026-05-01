---
description: Use Audio selectors (AudioSelectors) to specify a track or set of tracks from the input that you will use in your outputs. You can use multiple Audio selectors per input.
layout: schema
name: AudioSelector
properties_list:
- description: ''
  name: AudioDurationCorrection
  type: object
- description: ''
  name: CustomLanguageCode
  type: object
- description: ''
  name: DefaultSelection
  type: object
- description: ''
  name: ExternalAudioFileInput
  type: object
- description: ''
  name: HlsRenditionGroupSettings
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: Offset
  type: object
- description: ''
  name: Pids
  type: object
- description: ''
  name: ProgramSelection
  type: object
- description: ''
  name: RemixSettings
  type: object
- description: ''
  name: SelectorType
  type: object
- description: ''
  name: Tracks
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-selector-schema.json
slug: mediaconvert-api-audio-selector
source_filename: mediaconvert-api-audio-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-selector-schema.json\",\n  \"title\": \"AudioSelector\",\n  \"description\": \"Use Audio selectors (AudioSelectors) to specify a track or set of tracks from the input that you will use in your outputs. You can use multiple Audio selectors per input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDurationCorrection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioDurationCorrection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDurationCorrection\"\n          },\n          \"description\": \"Apply audio timing corrections to help synchronize audio and video in your output. To apply timing corrections, your input must meet the following requirements: * Container: MP4, or MOV, with an accurate time-to-sample\
  \ (STTS) table. * Audio track: AAC. Choose from the following audio timing correction settings: * Disabled (Default): Apply no correction. * Auto: Recommended for most inputs. MediaConvert analyzes the audio timing in your input and determines which correction setting to use, if needed. * Track: Adjust the duration of each audio frame by a constant amount to align the audio track length with STTS duration. Track-level correction does not affect pitch, and is recommended for tonal audio content such as music. * Frame: Adjust the duration of each audio frame by a variable amount to align audio frames with STTS timestamps. No corrections are made to already-aligned frames. Frame-level correction may affect the pitch of corrected frames, and is recommended for atonal audio content such as speech or percussion.\"\n        }\n      ]\n    },\n    \"CustomLanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin3Max3PatternAZaZ3\"\n        },\n \
  \       {\n          \"xml\": {\n            \"name\": \"customLanguageCode\"\n          },\n          \"description\": \"Selects a specific language code from within an audio source, using the ISO 639-2 or ISO 639-3 three-letter language code\"\n        }\n      ]\n    },\n    \"DefaultSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioDefaultSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"defaultSelection\"\n          },\n          \"description\": \"Enable this setting on one audio selector to set it as the default for the job. The service uses this default for outputs where it can't find the specified input audio. If you don't set a default, those outputs have no audio.\"\n        }\n      ]\n    },\n    \"ExternalAudioFileInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3Https\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"externalAudioFileInput\"\
  \n          },\n          \"description\": \"Specifies audio data from an external file source.\"\n        }\n      ]\n    },\n    \"HlsRenditionGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsRenditionGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsRenditionGroupSettings\"\n          },\n          \"description\": \"Settings specific to audio sources in an HLS alternate rendition group. Specify the properties (renditionGroupId, renditionName or renditionLanguageCode) to identify the unique audio track among the alternative rendition groups present in the HLS manifest. If no unique track is found, or multiple tracks match the properties provided, the job fails. If no properties in hlsRenditionGroupSettings are specified, the default audio track within the video segment is chosen. If there is no audio within video segment, the alternative audio with DEFAULT=YES is chosen instead.\"\n        }\n   \
  \   ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"Selects a specific language code from within an audio source.\"\n        }\n      ]\n    },\n    \"Offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offset\"\n          },\n          \"description\": \"Specifies a time delta in milliseconds to offset the audio from the input video.\"\n        }\n      ]\n    },\n    \"Pids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pids\"\n          },\n          \"description\": \"Selects a specific PID from\
  \ within an audio source (e.g. 257 selects PID 0x101).\"\n        }\n      ]\n    },\n    \"ProgramSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max8\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programSelection\"\n          },\n          \"description\": \"Use this setting for input streams that contain Dolby E, to have the service extract specific program data from the track. To select multiple programs, create multiple selectors with the same Track and different Program numbers. In the console, this setting is visible when you set Selector type to Track. Choose the program number from the dropdown list. If you are sending a JSON file, provide the program ID, which is part of the audio metadata. If your input file has incorrect metadata, you can choose All channels instead of a program number to have the service ignore the program IDs and include all the programs in the track.\"\n        }\n      ]\n\
  \    },\n    \"RemixSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemixSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remixSettings\"\n          },\n          \"description\": \"Use these settings to reorder the audio channels of one input to match those of another input. This allows you to combine the two files into a single output, one after the other.\"\n        }\n      ]\n    },\n    \"SelectorType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioSelectorType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"selectorType\"\n          },\n          \"description\": \"Specifies the type of the audio selector.\"\n        }\n      ]\n    },\n    \"Tracks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tracks\"\n   \
  \       },\n          \"description\": \"Identify a track from the input audio to include in this selector by entering the track index number. To include several tracks in a single audio selector, specify multiple tracks as follows. Using the console, enter a comma-separated list. For examle, type \\\"1,2,3\\\" to include tracks 1 through 3. Specifying directly in your JSON job file, provide the track numbers in an array. For example, \\\"tracks\\\": [1,2,3].\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-selector-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AudioSelector
---
