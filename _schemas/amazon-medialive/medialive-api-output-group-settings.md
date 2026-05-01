---
description: Output Group Settings
layout: schema
name: OutputGroupSettings
properties_list:
- description: ''
  name: ArchiveGroupSettings
  type: object
- description: ''
  name: FrameCaptureGroupSettings
  type: object
- description: ''
  name: HlsGroupSettings
  type: object
- description: ''
  name: MediaPackageGroupSettings
  type: object
- description: ''
  name: MsSmoothGroupSettings
  type: object
- description: ''
  name: MultiplexGroupSettings
  type: object
- description: ''
  name: RtmpGroupSettings
  type: object
- description: ''
  name: UdpGroupSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-output-group-settings-schema.json
slug: medialive-api-output-group-settings
source_filename: medialive-api-output-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-group-settings-schema.json\",\n  \"title\": \"OutputGroupSettings\",\n  \"description\": \"Output Group Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArchiveGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArchiveGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"archiveGroupSettings\"\n          }\n        }\n      ]\n    },\n    \"FrameCaptureGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"frameCaptureGroupSettings\"\n          }\n        }\n      ]\n    },\n    \"HlsGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/HlsGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsGroupSettings\"\n          }\n        }\n      ]\n    },\n    \"MediaPackageGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediaPackageGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaPackageGroupSettings\"\n          }\n        }\n      ]\n    },\n    \"MsSmoothGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"msSmoothGroupSettings\"\n          }\n        }\n      ]\n    },\n    \"MultiplexGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexGroupSettings\"\n          }\n        }\n      ]\n    },\n    \"RtmpGroupSettings\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RtmpGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rtmpGroupSettings\"\n          }\n        }\n      ]\n    },\n    \"UdpGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UdpGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"udpGroupSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: OutputGroupSettings
---
