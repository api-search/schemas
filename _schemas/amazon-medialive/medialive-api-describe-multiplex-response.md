---
description: Placeholder documentation for DescribeMultiplexResponse
layout: schema
name: DescribeMultiplexResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: Destinations
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: MultiplexSettings
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: PipelinesRunningCount
  type: object
- description: ''
  name: ProgramCount
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-describe-multiplex-response-schema.json
slug: medialive-api-describe-multiplex-response
source_filename: medialive-api-describe-multiplex-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-multiplex-response-schema.json\",\n  \"title\": \"DescribeMultiplexResponse\",\n  \"description\": \"Placeholder documentation for DescribeMultiplexResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The unique arn of the multiplex.\"\n        }\n      ]\n    },\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZones\"\n          },\n          \"description\": \"A list of availability zones for the multiplex.\"\
  \n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMultiplexOutputDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          },\n          \"description\": \"A list of the multiplex output destinations.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The unique id of the multiplex.\"\n        }\n      ]\n    },\n    \"MultiplexSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexSettings\"\n          },\n          \"description\": \"Configuration for a multiplex event.\"\n        }\n      ]\n    },\n    \"Name\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the multiplex.\"\n        }\n      ]\n    },\n    \"PipelinesRunningCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pipelinesRunningCount\"\n          },\n          \"description\": \"The number of currently healthy pipelines.\"\n        }\n      ]\n    },\n    \"ProgramCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programCount\"\n          },\n          \"description\": \"The number of programs in the multiplex.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexState\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"The current state of the multiplex.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-multiplex-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeMultiplexResponse
---
