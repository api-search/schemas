---
description: Output Settings
layout: schema
name: OutputSettings
properties_list:
- description: ''
  name: ArchiveOutputSettings
  type: object
- description: ''
  name: FrameCaptureOutputSettings
  type: object
- description: ''
  name: HlsOutputSettings
  type: object
- description: ''
  name: MediaPackageOutputSettings
  type: object
- description: ''
  name: MsSmoothOutputSettings
  type: object
- description: ''
  name: MultiplexOutputSettings
  type: object
- description: ''
  name: RtmpOutputSettings
  type: object
- description: ''
  name: UdpOutputSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-output-settings-schema.json
slug: medialive-api-output-settings
source_filename: medialive-api-output-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-settings-schema.json\",\n  \"title\": \"OutputSettings\",\n  \"description\": \"Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArchiveOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArchiveOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"archiveOutputSettings\"\n          }\n        }\n      ]\n    },\n    \"FrameCaptureOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"frameCaptureOutputSettings\"\n          }\n        }\n      ]\n    },\n    \"HlsOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsOutputSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsOutputSettings\"\n          }\n        }\n      ]\n    },\n    \"MediaPackageOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediaPackageOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaPackageOutputSettings\"\n          }\n        }\n      ]\n    },\n    \"MsSmoothOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"msSmoothOutputSettings\"\n          }\n        }\n      ]\n    },\n    \"MultiplexOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexOutputSettings\"\n          }\n        }\n      ]\n    },\n    \"RtmpOutputSettings\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RtmpOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rtmpOutputSettings\"\n          }\n        }\n      ]\n    },\n    \"UdpOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UdpOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"udpOutputSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: OutputSettings
---
