---
description: Placeholder documentation for OutputDestination
layout: schema
name: OutputDestination
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: MediaPackageSettings
  type: object
- description: ''
  name: MultiplexSettings
  type: object
- description: ''
  name: Settings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-output-destination-schema.json
slug: medialive-api-output-destination
source_filename: medialive-api-output-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-destination-schema.json\",\n  \"title\": \"OutputDestination\",\n  \"description\": \"Placeholder documentation for OutputDestination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"User-specified id. This is used in an output group or an output.\"\n        }\n      ]\n    },\n    \"MediaPackageSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaPackageOutputDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaPackageSettings\"\n          },\n          \"description\": \"\
  Destination settings for a MediaPackage output; one destination for both encoders.\"\n        }\n      ]\n    },\n    \"MultiplexSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexProgramChannelDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexSettings\"\n          },\n          \"description\": \"Destination settings for a Multiplex output; one destination for both encoders.\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"settings\"\n          },\n          \"description\": \"Destination settings for a standard output; one destination for each redundant encoder.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-destination-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputDestination
---
