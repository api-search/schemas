---
description: Global Configuration
layout: schema
name: GlobalConfiguration
properties_list:
- description: ''
  name: InitialAudioGain
  type: object
- description: ''
  name: InputEndAction
  type: object
- description: ''
  name: InputLossBehavior
  type: object
- description: ''
  name: OutputLockingMode
  type: object
- description: ''
  name: OutputTimingSource
  type: object
- description: ''
  name: SupportLowFramerateInputs
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-global-configuration-schema.json
slug: medialive-api-global-configuration
source_filename: medialive-api-global-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-global-configuration-schema.json\",\n  \"title\": \"GlobalConfiguration\",\n  \"description\": \"Global Configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InitialAudioGain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative60Max60\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"initialAudioGain\"\n          },\n          \"description\": \"Value to set the initial audio gain for the Live Event.\"\n        }\n      ]\n    },\n    \"InputEndAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlobalConfigurationInputEndAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputEndAction\"\n          },\n          \"description\": \"Indicates\
  \ the action to take when the current input completes (e.g. end-of-file). When switchAndLoopInputs is configured the encoder will restart at the beginning of the first input.  When \\\"none\\\" is configured the encoder will transcode either black, a solid color, or a user specified slate images per the \\\"Input Loss Behavior\\\" configuration until the next input switch occurs (which is controlled through the Channel Schedule API).\"\n        }\n      ]\n    },\n    \"InputLossBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLossBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossBehavior\"\n          },\n          \"description\": \"Settings for system actions when input is lost.\"\n        }\n      ]\n    },\n    \"OutputLockingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlobalConfigurationOutputLockingMode\"\n        },\n        {\n          \"xml\": {\n    \
  \        \"name\": \"outputLockingMode\"\n          },\n          \"description\": \"Indicates how MediaLive pipelines are synchronized.\\n\\nPIPELINE_LOCKING - MediaLive will attempt to synchronize the output of each pipeline to the other.\\nEPOCH_LOCKING - MediaLive will attempt to synchronize the output of each pipeline to the Unix epoch.\"\n        }\n      ]\n    },\n    \"OutputTimingSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlobalConfigurationOutputTimingSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputTimingSource\"\n          },\n          \"description\": \"Indicates whether the rate of frames emitted by the Live encoder should be paced by its system clock (which optionally may be locked to another source via NTP) or should be locked to the clock of the source that is providing the input stream.\"\n        }\n      ]\n    },\n    \"SupportLowFramerateInputs\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/GlobalConfigurationLowFramerateInputs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"supportLowFramerateInputs\"\n          },\n          \"description\": \"Adjusts video input buffer for streams with very low video framerates. This is commonly set to enabled for music channels with less than one video frame per second.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-global-configuration-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: GlobalConfiguration
---
