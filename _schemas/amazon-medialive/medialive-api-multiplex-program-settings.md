---
description: Multiplex Program settings configuration.
layout: schema
name: MultiplexProgramSettings
properties_list:
- description: ''
  name: PreferredChannelPipeline
  type: object
- description: ''
  name: ProgramNumber
  type: object
- description: ''
  name: ServiceDescriptor
  type: object
- description: ''
  name: VideoSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-program-settings-schema.json
slug: medialive-api-multiplex-program-settings
source_filename: medialive-api-multiplex-program-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-settings-schema.json\",\n  \"title\": \"MultiplexProgramSettings\",\n  \"description\": \"Multiplex Program settings configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PreferredChannelPipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PreferredChannelPipeline\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"preferredChannelPipeline\"\n          },\n          \"description\": \"Indicates which pipeline is preferred by the multiplex for program ingest.\"\n        }\n      ]\n    },\n    \"ProgramNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programNumber\"\n \
  \         },\n          \"description\": \"Unique program number.\"\n        }\n      ]\n    },\n    \"ServiceDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexProgramServiceDescriptor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceDescriptor\"\n          },\n          \"description\": \"Transport stream service descriptor configuration for the Multiplex program.\"\n        }\n      ]\n    },\n    \"VideoSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexVideoSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoSettings\"\n          },\n          \"description\": \"Program video settings configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProgramNumber\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MultiplexProgramSettings
---
