---
description: An HTTP Live Streaming (HLS) packaging configuration.
layout: schema
name: HlsPackage
properties_list:
- description: ''
  name: AdMarkers
  type: object
- description: ''
  name: AdTriggers
  type: object
- description: ''
  name: AdsOnDeliveryRestrictions
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: IncludeDvbSubtitles
  type: object
- description: ''
  name: IncludeIframeOnlyStream
  type: object
- description: ''
  name: PlaylistType
  type: object
- description: ''
  name: PlaylistWindowSeconds
  type: object
- description: ''
  name: ProgramDateTimeIntervalSeconds
  type: object
- description: ''
  name: SegmentDurationSeconds
  type: object
- description: ''
  name: StreamSelection
  type: object
- description: ''
  name: UseAudioRenditionGroup
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-hls-package-schema.json
slug: mediapackage-api-hls-package
source_filename: mediapackage-api-hls-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-package-schema.json\",\n  \"title\": \"HlsPackage\",\n  \"description\": \"An HTTP Live Streaming (HLS) packaging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdMarkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdMarkers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adMarkers\"\n          },\n          \"description\": \"This setting controls how ad markers are included in the packaged OriginEndpoint.\\n\\\"NONE\\\" will omit all SCTE-35 ad markers from the output.\\n\\\"PASSTHROUGH\\\" causes the manifest to contain a copy of the SCTE-35 ad\\nmarkers (comments) taken directly from the input HTTP Live Streaming (HLS) manifest.\\n\\\"SCTE35_ENHANCED\\\" generates ad markers and blackout tags\
  \ based on SCTE-35\\nmessages in the input source.\\n\\\"DATERANGE\\\" inserts EXT-X-DATERANGE tags to signal ad and program transition events \\nin HLS and CMAF manifests. For this option, you must set a programDateTimeIntervalSeconds value \\nthat is greater than 0.\\n\"\n        }\n      ]\n    },\n    \"AdTriggers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdTriggers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adTriggers\"\n          }\n        }\n      ]\n    },\n    \"AdsOnDeliveryRestrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdsOnDeliveryRestrictions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adsOnDeliveryRestrictions\"\n          }\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsEncryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  encryption\"\n          }\n        }\n      ]\n    },\n    \"IncludeDvbSubtitles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"includeDvbSubtitles\"\n          },\n          \"description\": \"When enabled, MediaPackage passes through digital video broadcasting (DVB) subtitles into the output.\"\n        }\n      ]\n    },\n    \"IncludeIframeOnlyStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"includeIframeOnlyStream\"\n          },\n          \"description\": \"When enabled, an I-Frame only stream will be included in the output.\"\n        }\n      ]\n    },\n    \"PlaylistType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaylistType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"playlistType\"\
  \n          },\n          \"description\": \"The HTTP Live Streaming (HLS) playlist type.\\nWhen either \\\"EVENT\\\" or \\\"VOD\\\" is specified, a corresponding EXT-X-PLAYLIST-TYPE\\nentry will be included in the media playlist.\\n\"\n        }\n      ]\n    },\n    \"PlaylistWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"playlistWindowSeconds\"\n          },\n          \"description\": \"Time window (in seconds) contained in each parent manifest.\"\n        }\n      ]\n    },\n    \"ProgramDateTimeIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programDateTimeIntervalSeconds\"\n          },\n          \"description\": \"The interval (in seconds) between each EXT-X-PROGRAM-DATE-TIME tag\\ninserted into manifests. Additionally, when\
  \ an interval is specified\\nID3Timed Metadata messages will be generated every 5 seconds using the\\ningest time of the content.\\nIf the interval is not specified, or set to 0, then\\nno EXT-X-PROGRAM-DATE-TIME tags will be inserted into manifests and no\\nID3Timed Metadata messages will be generated. Note that irrespective\\nof this parameter, if any ID3 Timed Metadata is found in HTTP Live Streaming (HLS) input,\\nit will be passed through to HLS output.\\n\"\n        }\n      ]\n    },\n    \"SegmentDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentDurationSeconds\"\n          },\n          \"description\": \"Duration (in seconds) of each fragment. Actual fragments will be\\nrounded to the nearest multiple of the source fragment duration.\\n\"\n        }\n      ]\n    },\n    \"StreamSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/StreamSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamSelection\"\n          }\n        }\n      ]\n    },\n    \"UseAudioRenditionGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"useAudioRenditionGroup\"\n          },\n          \"description\": \"When enabled, audio streams will be placed in rendition groups in the output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-package-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsPackage
---
