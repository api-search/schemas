---
description: Placeholder documentation for Input
layout: schema
name: Input
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: AttachedChannels
  type: object
- description: ''
  name: Destinations
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: InputClass
  type: object
- description: ''
  name: InputDevices
  type: object
- description: ''
  name: InputPartnerIds
  type: object
- description: ''
  name: InputSourceType
  type: object
- description: ''
  name: MediaConnectFlows
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: Sources
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-schema.json
slug: medialive-api-input
source_filename: medialive-api-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-schema.json\",\n  \"title\": \"Input\",\n  \"description\": \"Placeholder documentation for Input\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Unique ARN of the input (generated, immutable).\"\n        }\n      ]\n    },\n    \"AttachedChannels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attachedChannels\"\n          },\n          \"description\": \"A list of channel IDs that that input is attached to (currently an input can only be\
  \ attached to one channel).\"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          },\n          \"description\": \"A list of the destinations of the input (PUSH-type).\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The generated ID of the input (unique for user account, immutable).\"\n        }\n      ]\n    },\n    \"InputClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputClass\"\n          },\n          \"description\": \"STANDARD - MediaLive expects two sources to be\
  \ connected to this input. If the channel is also STANDARD, both sources will be ingested. If the channel is SINGLE_PIPELINE, only the first source will be ingested; the second source will always be ignored, even if the first source fails.\\nSINGLE_PIPELINE - You can connect only one source to this input. If the ChannelClass is also  SINGLE_PIPELINE, this value is valid. If the ChannelClass is STANDARD, this value is not valid because the channel requires two sources in the input.\\n\"\n        }\n      ]\n    },\n    \"InputDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputDeviceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputDevices\"\n          },\n          \"description\": \"Settings for the input devices.\"\n        }\n      ]\n    },\n    \"InputPartnerIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"inputPartnerIds\"\n          },\n          \"description\": \"A list of IDs for all Inputs which are partners of this one.\"\n        }\n      ]\n    },\n    \"InputSourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSourceType\"\n          },\n          \"description\": \"Certain pull input sources can be dynamic, meaning that they can have their URL's dynamically changes\\nduring input switch actions. Presently, this functionality only works with MP4_FILE and TS_FILE inputs.\\n\"\n        }\n      ]\n    },\n    \"MediaConnectFlows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaConnectFlow\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaConnectFlows\"\n          },\n          \"description\": \"A list of MediaConnect Flows for this input.\"\n        }\n\
  \      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The user-assigned name (This is a mutable value).\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the role this input assumes during and after creation.\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroups\"\n          },\n          \"description\": \"A list of IDs for all the Input Security Groups attached to the input.\"\n   \
  \     }\n      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"A list of the sources of the input (PULL-type).\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          }\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputType\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"type\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Input
---
