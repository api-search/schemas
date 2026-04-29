---
description: Resource configuration (codec, resolution, bitrate, ...)
layout: schema
name: ReservationResourceSpecification
properties_list:
- description: ''
  name: ChannelClass
  type: object
- description: ''
  name: Codec
  type: object
- description: ''
  name: MaximumBitrate
  type: object
- description: ''
  name: MaximumFramerate
  type: object
- description: ''
  name: Resolution
  type: object
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: SpecialFeature
  type: object
- description: ''
  name: VideoQuality
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-reservation-resource-specification-schema.json
slug: medialive-api-reservation-resource-specification
source_filename: medialive-api-reservation-resource-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reservation-resource-specification-schema.json\",\n  \"title\": \"ReservationResourceSpecification\",\n  \"description\": \"Resource configuration (codec, resolution, bitrate, ...)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelClass\"\n          },\n          \"description\": \"Channel class, e.g. 'STANDARD'\"\n        }\n      ]\n    },\n    \"Codec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationCodec\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codec\"\n          },\n          \"description\": \"Codec, e.g. 'AVC'\"\n       \
  \ }\n      ]\n    },\n    \"MaximumBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationMaximumBitrate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maximumBitrate\"\n          },\n          \"description\": \"Maximum bitrate, e.g. 'MAX_20_MBPS'\"\n        }\n      ]\n    },\n    \"MaximumFramerate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationMaximumFramerate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maximumFramerate\"\n          },\n          \"description\": \"Maximum framerate, e.g. 'MAX_30_FPS' (Outputs only)\"\n        }\n      ]\n    },\n    \"Resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationResolution\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resolution\"\n          },\n          \"description\": \"Resolution, e.g. 'HD'\"\n        }\n      ]\n    },\n\
  \    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationResourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceType\"\n          },\n          \"description\": \"Resource type, 'INPUT', 'OUTPUT', 'MULTIPLEX', or 'CHANNEL'\"\n        }\n      ]\n    },\n    \"SpecialFeature\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationSpecialFeature\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"specialFeature\"\n          },\n          \"description\": \"Special feature, e.g. 'AUDIO_NORMALIZATION' (Channels only)\"\n        }\n      ]\n    },\n    \"VideoQuality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationVideoQuality\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoQuality\"\n          },\n          \"description\": \"Video quality, e.g. 'STANDARD' (Outputs only)\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reservation-resource-specification-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ReservationResourceSpecification
---
