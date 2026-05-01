---
description: Holds the settings for a single schedule action.
layout: schema
name: ScheduleActionSettings
properties_list:
- description: ''
  name: HlsId3SegmentTaggingSettings
  type: object
- description: ''
  name: HlsTimedMetadataSettings
  type: object
- description: ''
  name: InputPrepareSettings
  type: object
- description: ''
  name: InputSwitchSettings
  type: object
- description: ''
  name: MotionGraphicsImageActivateSettings
  type: object
- description: ''
  name: MotionGraphicsImageDeactivateSettings
  type: object
- description: ''
  name: PauseStateSettings
  type: object
- description: ''
  name: Scte35InputSettings
  type: object
- description: ''
  name: Scte35ReturnToNetworkSettings
  type: object
- description: ''
  name: Scte35SpliceInsertSettings
  type: object
- description: ''
  name: Scte35TimeSignalSettings
  type: object
- description: ''
  name: StaticImageActivateSettings
  type: object
- description: ''
  name: StaticImageDeactivateSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-schedule-action-settings-schema.json
slug: medialive-api-schedule-action-settings
source_filename: medialive-api-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-schedule-action-settings-schema.json\",\n  \"title\": \"ScheduleActionSettings\",\n  \"description\": \"Holds the settings for a single schedule action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HlsId3SegmentTaggingSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsId3SegmentTaggingScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsId3SegmentTaggingSettings\"\n          },\n          \"description\": \"Action to insert HLS ID3 segment tagging\"\n        }\n      ]\n    },\n    \"HlsTimedMetadataSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsTimedMetadataScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"hlsTimedMetadataSettings\"\n          },\n          \"description\": \"Action to insert HLS metadata\"\n        }\n      ]\n    },\n    \"InputPrepareSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputPrepareScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputPrepareSettings\"\n          },\n          \"description\": \"Action to prepare an input for a future immediate input switch\"\n        }\n      ]\n    },\n    \"InputSwitchSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSwitchScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSwitchSettings\"\n          },\n          \"description\": \"Action to switch the input\"\n        }\n      ]\n    },\n    \"MotionGraphicsImageActivateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionGraphicsActivateScheduleActionSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"motionGraphicsImageActivateSettings\"\n          },\n          \"description\": \"Action to activate a motion graphics image overlay\"\n        }\n      ]\n    },\n    \"MotionGraphicsImageDeactivateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionGraphicsDeactivateScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"motionGraphicsImageDeactivateSettings\"\n          },\n          \"description\": \"Action to deactivate a motion graphics image overlay\"\n        }\n      ]\n    },\n    \"PauseStateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PauseStateScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pauseStateSettings\"\n          },\n          \"description\": \"Action to pause or unpause one or both channel pipelines\"\n        }\n      ]\n\
  \    },\n    \"Scte35InputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35InputScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35InputSettings\"\n          },\n          \"description\": \"Action to specify scte35 input\"\n        }\n      ]\n    },\n    \"Scte35ReturnToNetworkSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35ReturnToNetworkScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35ReturnToNetworkSettings\"\n          },\n          \"description\": \"Action to insert SCTE-35 return_to_network message\"\n        }\n      ]\n    },\n    \"Scte35SpliceInsertSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35SpliceInsertScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35SpliceInsertSettings\"\n    \
  \      },\n          \"description\": \"Action to insert SCTE-35 splice_insert message\"\n        }\n      ]\n    },\n    \"Scte35TimeSignalSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35TimeSignalScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35TimeSignalSettings\"\n          },\n          \"description\": \"Action to insert SCTE-35 time_signal message\"\n        }\n      ]\n    },\n    \"StaticImageActivateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StaticImageActivateScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"staticImageActivateSettings\"\n          },\n          \"description\": \"Action to activate a static image overlay\"\n        }\n      ]\n    },\n    \"StaticImageDeactivateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StaticImageDeactivateScheduleActionSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"staticImageDeactivateSettings\"\n          },\n          \"description\": \"Action to deactivate a static image overlay\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-schedule-action-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ScheduleActionSettings
---
