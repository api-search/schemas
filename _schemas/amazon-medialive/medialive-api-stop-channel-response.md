---
description: Placeholder documentation for StopChannelResponse
layout: schema
name: StopChannelResponse
properties_list:
- description: ''
  name: Arn
  type: object
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
  name: EgressEndpoints
  type: object
- description: ''
  name: EncoderSettings
  type: object
- description: ''
  name: Id
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
  name: PipelineDetails
  type: object
- description: ''
  name: PipelinesRunningCount
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Vpc
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-stop-channel-response-schema.json
slug: medialive-api-stop-channel-response
source_filename: medialive-api-stop-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-stop-channel-response-schema.json\",\n  \"title\": \"StopChannelResponse\",\n  \"description\": \"Placeholder documentation for StopChannelResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The unique arn of the channel.\"\n        }\n      ]\n    },\n    \"CdiInputSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CdiInputSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cdiInputSpecification\"\n          },\n          \"description\": \"Specification of CDI inputs for this channel\"\n\
  \        }\n      ]\n    },\n    \"ChannelClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelClass\"\n          },\n          \"description\": \"The class for this channel. STANDARD for a channel with two pipelines or SINGLE_PIPELINE for a channel with one pipeline.\"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          },\n          \"description\": \"A list of destinations of the channel. For UDP outputs, there is one\\ndestination per output. For other types (HLS, for example), there is\\none destination per packager.\\n\"\n        }\n      ]\n    },\n    \"EgressEndpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfChannelEgressEndpoint\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"egressEndpoints\"\n          },\n          \"description\": \"The endpoints where outgoing connections initiate from\"\n        }\n      ]\n    },\n    \"EncoderSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncoderSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encoderSettings\"\n          }\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The unique id of the channel.\"\n        }\n      ]\n    },\n    \"InputAttachments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputAttachment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputAttachments\"\n          },\n          \"description\"\
  : \"List of input attachments for channel.\"\n        }\n      ]\n    },\n    \"InputSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSpecification\"\n          },\n          \"description\": \"Specification of network and file inputs for this channel\"\n        }\n      ]\n    },\n    \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logLevel\"\n          },\n          \"description\": \"The log level being written to CloudWatch Logs.\"\n        }\n      ]\n    },\n    \"Maintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenance\"\n          },\n          \"description\": \"Maintenance settings\
  \ for this channel.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the channel. (user-mutable)\"\n        }\n      ]\n    },\n    \"PipelineDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfPipelineDetail\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pipelineDetails\"\n          },\n          \"description\": \"Runtime details for the pipelines of a running channel.\"\n        }\n      ]\n    },\n    \"PipelinesRunningCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pipelinesRunningCount\"\n          },\n          \"description\": \"The number of currently healthy pipelines.\"\n    \
  \    }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the role assumed when running the Channel.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          }\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    },\n    \"Vpc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcOutputSettingsDescription\"\n     \
  \   },\n        {\n          \"xml\": {\n            \"name\": \"vpc\"\n          },\n          \"description\": \"Settings for VPC output\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-stop-channel-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StopChannelResponse
---
