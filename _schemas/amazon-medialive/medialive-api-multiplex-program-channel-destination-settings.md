---
description: Multiplex Program Input Destination Settings for outputting a Channel to a Multiplex
layout: schema
name: MultiplexProgramChannelDestinationSettings
properties_list:
- description: ''
  name: MultiplexId
  type: object
- description: ''
  name: ProgramName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-program-channel-destination-settings-schema.json
slug: medialive-api-multiplex-program-channel-destination-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-channel-destination-settings-schema.json\",\n  \"title\": \"MultiplexProgramChannelDestinationSettings\",\n  \"description\": \"Multiplex Program Input Destination Settings for outputting a Channel to a Multiplex\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MultiplexId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexId\"\n          },\n          \"description\": \"The ID of the Multiplex that the encoder is providing output to. You do not need to specify the individual inputs to the Multiplex; MediaLive will handle the connection of the two MediaLive pipelines to the two Multiplex instances.\\nThe Multiplex must be in the same region as\
  \ the Channel.\"\n        }\n      ]\n    },\n    \"ProgramName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programName\"\n          },\n          \"description\": \"The program name of the Multiplex program that the encoder is providing output to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-channel-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexProgramChannelDestinationSettings
---
