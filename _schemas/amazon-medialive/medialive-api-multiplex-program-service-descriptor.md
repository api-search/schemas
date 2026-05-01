---
description: Transport stream service descriptor configuration for the Multiplex program.
layout: schema
name: MultiplexProgramServiceDescriptor
properties_list:
- description: ''
  name: ProviderName
  type: object
- description: ''
  name: ServiceName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-program-service-descriptor-schema.json
slug: medialive-api-multiplex-program-service-descriptor
source_filename: medialive-api-multiplex-program-service-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-service-descriptor-schema.json\",\n  \"title\": \"MultiplexProgramServiceDescriptor\",\n  \"description\": \"Transport stream service descriptor configuration for the Multiplex program.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"providerName\"\n          },\n          \"description\": \"Name of the provider.\"\n        }\n      ]\n    },\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceName\"\n          },\n          \"description\": \"Name\
  \ of the service.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProviderName\",\n    \"ServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-service-descriptor-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MultiplexProgramServiceDescriptor
---
