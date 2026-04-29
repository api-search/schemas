---
description: An array of settings that describes characteristics of a network profile.
layout: schema
name: NetworkProfile
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: uplinkBandwidthBits
  type: object
- description: ''
  name: downlinkBandwidthBits
  type: object
- description: ''
  name: uplinkDelayMs
  type: object
- description: ''
  name: downlinkDelayMs
  type: object
- description: ''
  name: uplinkJitterMs
  type: object
- description: ''
  name: downlinkJitterMs
  type: object
- description: ''
  name: uplinkLossPercent
  type: object
- description: ''
  name: downlinkLossPercent
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-network-profile-schema.json
slug: amazon-device-farm-network-profile
source_filename: amazon-device-farm-network-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-network-profile-schema.json\",\n  \"title\": \"NetworkProfile\",\n  \"description\": \"An array of settings that describes characteristics of a network profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the network profile.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the network profile.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n     \
  \   },\n        {\n          \"description\": \"The description of the network profile.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkProfileType\"\n        },\n        {\n          \"description\": \"The type of network profile. Valid values are listed here.\"\n        }\n      ]\n    },\n    \"uplinkBandwidthBits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The data throughput rate in bits per second, as an integer from 0 to 104857600.\"\n        }\n      ]\n    },\n    \"downlinkBandwidthBits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The data throughput rate in bits per second, as an integer from 0 to 104857600.\"\n        }\n      ]\n    },\n    \"uplinkDelayMs\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"Delay time for all packets to destination in milliseconds as an integer from 0 to 2000.\"\n        }\n      ]\n    },\n    \"downlinkDelayMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"Delay time for all packets to destination in milliseconds as an integer from 0 to 2000.\"\n        }\n      ]\n    },\n    \"uplinkJitterMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"Time variation in the delay of received packets in milliseconds as an integer from 0 to 2000.\"\n        }\n      ]\n    },\n    \"downlinkJitterMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"Time variation in the delay of received packets in milliseconds\
  \ as an integer from 0 to 2000.\"\n        }\n      ]\n    },\n    \"uplinkLossPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PercentInteger\"\n        },\n        {\n          \"description\": \"Proportion of transmitted packets that fail to arrive from 0 to 100 percent.\"\n        }\n      ]\n    },\n    \"downlinkLossPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PercentInteger\"\n        },\n        {\n          \"description\": \"Proportion of received packets that fail to arrive from 0 to 100 percent.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-network-profile-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: NetworkProfile
---
