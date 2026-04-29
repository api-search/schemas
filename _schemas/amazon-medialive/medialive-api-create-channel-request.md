---
description: A request to create a channel
layout: schema
name: CreateChannelRequest
properties_list:
- description: ''
  name: CdiInputSpecification
  type: object
- description: ''
  name: ChannelClass
  type: object
- description: ''
  name: Destinations
  type: object
- description: ''
  name: EncoderSettings
  type: object
- description: ''
  name: InputAttachments
  type: object
- description: ''
  name: InputSpecification
  type: object
- description: ''
  name: LogLevel
  type: object
- description: ''
  name: Maintenance
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RequestId
  type: object
- description: ''
  name: Reserved
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Vpc
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-create-channel-request-schema.json
slug: medialive-api-create-channel-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-channel-request-schema.json\",\n  \"title\": \"CreateChannelRequest\",\n  \"description\": \"A request to create a channel\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CdiInputSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CdiInputSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cdiInputSpecification\"\n          },\n          \"description\": \"Specification of CDI inputs for this channel\"\n        }\n      ]\n    },\n    \"ChannelClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelClass\"\n          },\n          \"description\": \"The class for this channel. STANDARD\
  \ for a channel with two pipelines or SINGLE_PIPELINE for a channel with one pipeline.\"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          }\n        }\n      ]\n    },\n    \"EncoderSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncoderSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encoderSettings\"\n          }\n        }\n      ]\n    },\n    \"InputAttachments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputAttachment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputAttachments\"\n          },\n          \"description\": \"List of input attachments for channel.\"\n        }\n      ]\n    },\n    \"InputSpecification\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/InputSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSpecification\"\n          },\n          \"description\": \"Specification of network and file inputs for this channel\"\n        }\n      ]\n    },\n    \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logLevel\"\n          },\n          \"description\": \"The log level to write to CloudWatch Logs.\"\n        }\n      ]\n    },\n    \"Maintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceCreateSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenance\"\n          },\n          \"description\": \"Maintenance settings for this channel.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of channel.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"requestId\"\n          },\n          \"description\": \"Unique request ID to be specified. This is needed to prevent retries from\\ncreating multiple resources.\\n\"\n        }\n      ]\n    },\n    \"Reserved\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"reserved\"\n          },\n          \"description\": \"Deprecated field that's only usable by whitelisted customers.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"An optional Amazon Resource Name (ARN) of the role to assume when running the Channel.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    },\n    \"Vpc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpc\"\n          },\n          \"description\": \"Settings for the VPC outputs\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-channel-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateChannelRequest
---
