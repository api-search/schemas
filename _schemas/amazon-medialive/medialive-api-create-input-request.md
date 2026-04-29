---
description: The name of the input
layout: schema
name: CreateInputRequest
properties_list:
- description: ''
  name: Destinations
  type: object
- description: ''
  name: InputDevices
  type: object
- description: ''
  name: InputSecurityGroups
  type: object
- description: ''
  name: MediaConnectFlows
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RequestId
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Sources
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Vpc
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-create-input-request-schema.json
slug: medialive-api-create-input-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-input-request-schema.json\",\n  \"title\": \"CreateInputRequest\",\n  \"description\": \"The name of the input\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputDestinationRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          },\n          \"description\": \"Destination settings for PUSH type inputs.\"\n        }\n      ]\n    },\n    \"InputDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputDeviceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputDevices\"\n          },\n          \"description\": \"Settings for the devices.\"\n      \
  \  }\n      ]\n    },\n    \"InputSecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSecurityGroups\"\n          },\n          \"description\": \"A list of security groups referenced by IDs to attach to the input.\"\n        }\n      ]\n    },\n    \"MediaConnectFlows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaConnectFlowRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaConnectFlows\"\n          },\n          \"description\": \"A list of the MediaConnect Flows that you want to use in this input. You can specify as few as one\\nFlow and presently, as many as two. The only requirement is when you have more than one is that each Flow is in a\\nseparate Availability Zone as this ensures your EML input is redundant to AZ issues.\\n\"\n        }\n      ]\n    },\n    \"Name\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of the input.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"requestId\"\n          },\n          \"description\": \"Unique identifier of the request to ensure the request is handled\\nexactly once in case of retries.\\n\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the role this input assumes during and after creation.\"\n        }\n      ]\n    },\n    \"Sources\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"The source URLs for a PULL-type input. Every PULL type input needs\\nexactly two source URLs for redundancy.\\nOnly specify sources for PULL type Inputs. Leave Destinations empty.\\n\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          }\n        }\n      ]\n    },\n    \"Vpc\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/InputVpcRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpc\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-input-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateInputRequest
---
