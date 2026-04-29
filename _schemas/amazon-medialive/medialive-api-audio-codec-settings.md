---
description: Audio Codec Settings
layout: schema
name: AudioCodecSettings
properties_list:
- description: ''
  name: AacSettings
  type: object
- description: ''
  name: Ac3Settings
  type: object
- description: ''
  name: Eac3AtmosSettings
  type: object
- description: ''
  name: Eac3Settings
  type: object
- description: ''
  name: Mp2Settings
  type: object
- description: ''
  name: PassThroughSettings
  type: object
- description: ''
  name: WavSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-codec-settings-schema.json
slug: medialive-api-audio-codec-settings
source_filename: medialive-api-audio-codec-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-codec-settings-schema.json\",\n  \"title\": \"AudioCodecSettings\",\n  \"description\": \"Audio Codec Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AacSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"aacSettings\"\n          }\n        }\n      ]\n    },\n    \"Ac3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ac3Settings\"\n          }\n        }\n      ]\n    },\n    \"Eac3AtmosSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosSettings\"\n        },\n        {\n      \
  \    \"xml\": {\n            \"name\": \"eac3AtmosSettings\"\n          }\n        }\n      ]\n    },\n    \"Eac3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eac3Settings\"\n          }\n        }\n      ]\n    },\n    \"Mp2Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp2Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mp2Settings\"\n          }\n        }\n      ]\n    },\n    \"PassThroughSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PassThroughSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passThroughSettings\"\n          }\n        }\n      ]\n    },\n    \"WavSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WavSettings\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"wavSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-codec-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioCodecSettings
---
