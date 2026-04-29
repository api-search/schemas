---
description: A request to create a multiplex.
layout: schema
name: CreateMultiplexRequest
properties_list:
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: MultiplexSettings
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RequestId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-create-multiplex-request-schema.json
slug: medialive-api-create-multiplex-request
source_filename: medialive-api-create-multiplex-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-multiplex-request-schema.json\",\n  \"title\": \"CreateMultiplexRequest\",\n  \"description\": \"A request to create a multiplex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZones\"\n          },\n          \"description\": \"A list of availability zones for the multiplex. You must specify exactly two.\"\n        }\n      ]\n    },\n    \"MultiplexSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexSettings\"\n          },\n          \"description\"\
  : \"Configuration for a multiplex event.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of multiplex.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"requestId\"\n          },\n          \"description\": \"Unique request ID. This prevents retries from creating multiple\\nresources.\\n\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n   \
  \ \"RequestId\",\n    \"MultiplexSettings\",\n    \"AvailabilityZones\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-multiplex-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateMultiplexRequest
---
