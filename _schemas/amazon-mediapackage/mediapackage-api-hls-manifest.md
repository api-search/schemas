---
description: A HTTP Live Streaming (HLS) manifest configuration.
layout: schema
name: HlsManifest
properties_list:
- description: ''
  name: AdMarkers
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: IncludeIframeOnlyStream
  type: object
- description: ''
  name: ManifestName
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
  name: Url
  type: object
- description: ''
  name: AdTriggers
  type: object
- description: ''
  name: AdsOnDeliveryRestrictions
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-hls-manifest-schema.json
slug: mediapackage-api-hls-manifest
source_filename: mediapackage-api-hls-manifest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-manifest-schema.json\",\n  \"title\": \"HlsManifest\",\n  \"description\": \"A HTTP Live Streaming (HLS) manifest configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdMarkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdMarkers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adMarkers\"\n          },\n          \"description\": \"This setting controls how ad markers are included in the packaged OriginEndpoint.\\n\\\"NONE\\\" will omit all SCTE-35 ad markers from the output.\\n\\\"PASSTHROUGH\\\" causes the manifest to contain a copy of the SCTE-35 ad\\nmarkers (comments) taken directly from the input HTTP Live Streaming (HLS) manifest.\\n\\\"SCTE35_ENHANCED\\\" generates ad markers and blackout tags\
  \ based on SCTE-35\\nmessages in the input source.\\n\\\"DATERANGE\\\" inserts EXT-X-DATERANGE tags to signal ad and program transition events \\nin HLS and CMAF manifests. For this option, you must set a programDateTimeIntervalSeconds value \\nthat is greater than 0.\\n\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The ID of the manifest. The ID must be unique within the OriginEndpoint and it cannot be changed after it is created.\"\n        }\n      ]\n    },\n    \"IncludeIframeOnlyStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"includeIframeOnlyStream\"\n          },\n          \"description\": \"When enabled, an I-Frame only stream will be included in the output.\"\
  \n        }\n      ]\n    },\n    \"ManifestName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestName\"\n          },\n          \"description\": \"An optional short string appended to the end of the OriginEndpoint URL. If not specified, defaults to the manifestName for the OriginEndpoint.\"\n        }\n      ]\n    },\n    \"PlaylistType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaylistType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"playlistType\"\n          },\n          \"description\": \"The HTTP Live Streaming (HLS) playlist type.\\nWhen either \\\"EVENT\\\" or \\\"VOD\\\" is specified, a corresponding EXT-X-PLAYLIST-TYPE\\nentry will be included in the media playlist.\\n\"\n        }\n      ]\n    },\n    \"PlaylistWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"playlistWindowSeconds\"\n          },\n          \"description\": \"Time window (in seconds) contained in each parent manifest.\"\n        }\n      ]\n    },\n    \"ProgramDateTimeIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programDateTimeIntervalSeconds\"\n          },\n          \"description\": \"The interval (in seconds) between each EXT-X-PROGRAM-DATE-TIME tag\\ninserted into manifests. Additionally, when an interval is specified\\nID3Timed Metadata messages will be generated every 5 seconds using the\\ningest time of the content.\\nIf the interval is not specified, or set to 0, then\\nno EXT-X-PROGRAM-DATE-TIME tags will be inserted into manifests and no\\nID3Timed Metadata messages will be generated. Note that irrespective\\nof this parameter, if any ID3 Timed Metadata is found\
  \ in HTTP Live Streaming (HLS) input,\\nit will be passed through to HLS output.\\n\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"The URL of the packaged OriginEndpoint for consumption.\"\n        }\n      ]\n    },\n    \"AdTriggers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdTriggers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adTriggers\"\n          }\n        }\n      ]\n    },\n    \"AdsOnDeliveryRestrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdsOnDeliveryRestrictions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adsOnDeliveryRestrictions\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-manifest-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsManifest
---
