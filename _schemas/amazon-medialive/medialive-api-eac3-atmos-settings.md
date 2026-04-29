---
description: Eac3 Atmos Settings
layout: schema
name: Eac3AtmosSettings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: CodingMode
  type: object
- description: ''
  name: Dialnorm
  type: object
- description: ''
  name: DrcLine
  type: object
- description: ''
  name: DrcRf
  type: object
- description: ''
  name: HeightTrim
  type: object
- description: ''
  name: SurroundTrim
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-eac3-atmos-settings-schema.json
slug: medialive-api-eac3-atmos-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-eac3-atmos-settings-schema.json\",\n  \"title\": \"Eac3AtmosSettings\",\n  \"description\": \"Eac3 Atmos Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Average bitrate in bits/second. Valid bitrates depend on the coding mode.\\n//  * @affectsRightSizing true\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosCodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"Dolby Digital Plus with\
  \ Dolby Atmos coding mode. Determines number of channels.\"\n        }\n      ]\n    },\n    \"Dialnorm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max31\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dialnorm\"\n          },\n          \"description\": \"Sets the dialnorm for the output. Default 23.\"\n        }\n      ]\n    },\n    \"DrcLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosDrcLine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"drcLine\"\n          },\n          \"description\": \"Sets the Dolby dynamic range compression profile.\"\n        }\n      ]\n    },\n    \"DrcRf\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AtmosDrcRf\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"drcRf\"\n          },\n          \"description\": \"Sets the profile for heavy Dolby dynamic range\
  \ compression, ensures that the instantaneous signal peaks do not exceed specified levels.\"\n        }\n      ]\n    },\n    \"HeightTrim\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"heightTrim\"\n          },\n          \"description\": \"Height dimensional trim. Sets the maximum amount to attenuate the height channels when the downstream player isn??t configured to handle Dolby Digital Plus with Dolby Atmos and must remix the channels.\"\n        }\n      ]\n    },\n    \"SurroundTrim\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"surroundTrim\"\n          },\n          \"description\": \"Surround dimensional trim. Sets the maximum amount to attenuate the surround channels when the downstream player isn't configured to handle Dolby Digital Plus with Dolby Atmos\
  \ and must remix the channels.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-eac3-atmos-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3AtmosSettings
---
