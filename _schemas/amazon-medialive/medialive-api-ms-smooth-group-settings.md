---
description: Ms Smooth Group Settings
layout: schema
name: MsSmoothGroupSettings
properties_list:
- description: ''
  name: AcquisitionPointId
  type: object
- description: ''
  name: AudioOnlyTimecodeControl
  type: object
- description: ''
  name: CertificateMode
  type: object
- description: ''
  name: ConnectionRetryInterval
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: EventId
  type: object
- description: ''
  name: EventIdMode
  type: object
- description: ''
  name: EventStopBehavior
  type: object
- description: ''
  name: FilecacheDuration
  type: object
- description: ''
  name: FragmentLength
  type: object
- description: ''
  name: InputLossAction
  type: object
- description: ''
  name: NumRetries
  type: object
- description: ''
  name: RestartDelay
  type: object
- description: ''
  name: SegmentationMode
  type: object
- description: ''
  name: SendDelayMs
  type: object
- description: ''
  name: SparseTrackType
  type: object
- description: ''
  name: StreamManifestBehavior
  type: object
- description: ''
  name: TimestampOffset
  type: object
- description: ''
  name: TimestampOffsetMode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-ms-smooth-group-settings-schema.json
slug: medialive-api-ms-smooth-group-settings
source_filename: medialive-api-ms-smooth-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ms-smooth-group-settings-schema.json\",\n  \"title\": \"MsSmoothGroupSettings\",\n  \"description\": \"Ms Smooth Group Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcquisitionPointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"acquisitionPointId\"\n          },\n          \"description\": \"The ID to include in each message in the sparse track. Ignored if sparseTrackType is NONE.\"\n        }\n      ]\n    },\n    \"AudioOnlyTimecodeControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmoothGroupAudioOnlyTimecodeControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioOnlyTimecodeControl\"\n\
  \          },\n          \"description\": \"If set to passthrough for an audio-only MS Smooth output, the fragment absolute time will be set to the current timecode. This option does not write timecodes to the audio elementary stream.\"\n        }\n      ]\n    },\n    \"CertificateMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmoothGroupCertificateMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"certificateMode\"\n          },\n          \"description\": \"If set to verifyAuthenticity, verify the https certificate chain to a trusted Certificate Authority (CA).  This will cause https outputs to self-signed certificates to fail.\"\n        }\n      ]\n    },\n    \"ConnectionRetryInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"connectionRetryInterval\"\n          },\n          \"description\": \"\
  Number of seconds to wait before retrying connection to the IIS server if the connection is lost. Content will be cached during this time and the cache will be be delivered to the IIS server once the connection is re-established.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocationRef\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"Smooth Streaming publish point on an IIS server. Elemental Live acts as a \\\"Push\\\" encoder to IIS.\"\n        }\n      ]\n    },\n    \"EventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eventId\"\n          },\n          \"description\": \"MS Smooth event ID to be sent to the IIS server.\\n\\nShould only be specified if eventIdMode is set to useConfigured.\"\n       \
  \ }\n      ]\n    },\n    \"EventIdMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmoothGroupEventIdMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eventIdMode\"\n          },\n          \"description\": \"Specifies whether or not to send an event ID to the IIS server. If no event ID is sent and the same Live Event is used without changing the publishing point, clients might see cached video from the previous run.\\n\\nOptions:\\n- \\\"useConfigured\\\" - use the value provided in eventId\\n- \\\"useTimestamp\\\" - generate and send an event ID based on the current timestamp\\n- \\\"noEventId\\\" - do not send an event ID to the IIS server.\"\n        }\n      ]\n    },\n    \"EventStopBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmoothGroupEventStopBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eventStopBehavior\"\n          },\n          \"\
  description\": \"When set to sendEos, send EOS signal to IIS server when stopping the event\"\n        }\n      ]\n    },\n    \"FilecacheDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filecacheDuration\"\n          },\n          \"description\": \"Size in seconds of file cache for streaming outputs.\"\n        }\n      ]\n    },\n    \"FragmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fragmentLength\"\n          },\n          \"description\": \"Length of mp4 fragments to generate (in seconds). Fragment length must be compatible with GOP size and framerate.\"\n        }\n      ]\n    },\n    \"InputLossAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLossActionForMsSmoothOut\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"inputLossAction\"\n          },\n          \"description\": \"Parameter that control output group behavior on input loss.\"\n        }\n      ]\n    },\n    \"NumRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numRetries\"\n          },\n          \"description\": \"Number of retry attempts.\"\n        }\n      ]\n    },\n    \"RestartDelay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"restartDelay\"\n          },\n          \"description\": \"Number of seconds before initiating a restart due to output failure, due to exhausting the numRetries on one segment, or exceeding filecacheDuration.\"\n        }\n      ]\n    },\n    \"SegmentationMode\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/SmoothGroupSegmentationMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationMode\"\n          },\n          \"description\": \"useInputSegmentation has been deprecated. The configured segment size is always used.\"\n        }\n      ]\n    },\n    \"SendDelayMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max10000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sendDelayMs\"\n          },\n          \"description\": \"Number of milliseconds to delay the output from the second pipeline.\"\n        }\n      ]\n    },\n    \"SparseTrackType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmoothGroupSparseTrackType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sparseTrackType\"\n          },\n          \"description\": \"Identifies the type of data to place in the sparse track:\\n- SCTE35:\
  \ Insert SCTE-35 messages from the source content. With each message, insert an IDR frame to start a new segment.\\n- SCTE35_WITHOUT_SEGMENTATION: Insert SCTE-35 messages from the source content. With each message, insert an IDR frame but don't start a new segment.\\n- NONE: Don't generate a sparse track for any outputs in this output group.\"\n        }\n      ]\n    },\n    \"StreamManifestBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmoothGroupStreamManifestBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamManifestBehavior\"\n          },\n          \"description\": \"When set to send, send stream manifest so publishing point doesn't start until all streams start.\"\n        }\n      ]\n    },\n    \"TimestampOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timestampOffset\"\n         \
  \ },\n          \"description\": \"Timestamp offset for the event.  Only used if timestampOffsetMode is set to useConfiguredOffset.\"\n        }\n      ]\n    },\n    \"TimestampOffsetMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmoothGroupTimestampOffsetMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timestampOffsetMode\"\n          },\n          \"description\": \"Type of timestamp date offset to use.\\n- useEventStartDate: Use the date the event was started as the offset\\n- useConfiguredOffset: Use an explicitly configured date as the offset\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ms-smooth-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MsSmoothGroupSettings
---
