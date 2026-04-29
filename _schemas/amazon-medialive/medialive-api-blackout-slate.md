---
description: Blackout Slate
layout: schema
name: BlackoutSlate
properties_list:
- description: ''
  name: BlackoutSlateImage
  type: object
- description: ''
  name: NetworkEndBlackout
  type: object
- description: ''
  name: NetworkEndBlackoutImage
  type: object
- description: ''
  name: NetworkId
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-blackout-slate-schema.json
slug: medialive-api-blackout-slate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-blackout-slate-schema.json\",\n  \"title\": \"BlackoutSlate\",\n  \"description\": \"Blackout Slate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlackoutSlateImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blackoutSlateImage\"\n          },\n          \"description\": \"Blackout slate image to be used. Leave empty for solid black. Only bmp and png images are supported.\"\n        }\n      ]\n    },\n    \"NetworkEndBlackout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlackoutSlateNetworkEndBlackout\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkEndBlackout\"\n          },\n          \"description\"\
  : \"Setting to enabled causes the encoder to blackout the video, audio, and captions, and raise the \\\"Network Blackout Image\\\" slate when an SCTE104/35 Network End Segmentation Descriptor is encountered. The blackout will be lifted when the Network Start Segmentation Descriptor is encountered. The Network End and Network Start descriptors must contain a network ID that matches the value entered in \\\"Network ID\\\".\"\n        }\n      ]\n    },\n    \"NetworkEndBlackoutImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkEndBlackoutImage\"\n          },\n          \"description\": \"Path to local file to use as Network End Blackout image. Image will be scaled to fill the entire output raster.\"\n        }\n      ]\n    },\n    \"NetworkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin34Max34\"\n        },\n    \
  \    {\n          \"xml\": {\n            \"name\": \"networkId\"\n          },\n          \"description\": \"Provides Network ID that matches EIDR ID format (e.g., \\\"10.XXXX/XXXX-XXXX-XXXX-XXXX-XXXX-C\\\").\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlackoutSlateState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"When set to enabled, causes video, audio and captions to be blanked when indicated by program metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-blackout-slate-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BlackoutSlate
---
