---
description: The settings for an output.
layout: schema
name: Output
properties_list:
- description: ''
  name: DataTransferSubscriberFeePercent
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: EntitlementArn
  type: object
- description: ''
  name: ListenerAddress
  type: object
- description: ''
  name: MediaLiveInputArn
  type: object
- description: ''
  name: MediaStreamOutputConfigurations
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: OutputArn
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: Transport
  type: object
- description: ''
  name: VpcInterfaceAttachment
  type: object
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: BridgePorts
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-output-schema.json
slug: mediaconnect-api-output
source_filename: mediaconnect-api-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-output-schema.json\",\n  \"title\": \"Output\",\n  \"description\": \"The settings for an output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataTransferSubscriberFeePercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataTransferSubscriberFeePercent\"\n          },\n          \"description\": \"Percentage from 0-100 of the data transfer cost to be billed to the subscriber.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A description of\
  \ the output.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"The address where you want to send the output.\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          },\n          \"description\": \"The type of key used for the encryption. If no keyType is provided, the service will use the default setting (static-key).\"\n        }\n      ]\n    },\n    \"EntitlementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementArn\"\n          },\n          \"description\": \"The ARN\
  \ of the entitlement on the originator''s flow. This value is relevant only on entitled flows.\"\n        }\n      ]\n    },\n    \"ListenerAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"listenerAddress\"\n          },\n          \"description\": \"The IP address that the receiver requires in order to establish a connection with the flow. For public networking, the ListenerAddress is represented by the elastic IP address of the flow. For private networking, the ListenerAddress is represented by the elastic network interface IP address of the VPC. This field applies only to outputs that use the Zixi pull or SRT listener protocol.\"\n        }\n      ]\n    },\n    \"MediaLiveInputArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaLiveInputArn\"\n   \
  \       },\n          \"description\": \"The input ARN of the AWS Elemental MediaLive channel. This parameter is relevant only for outputs that were added by creating a MediaLive input.\"\n        }\n      ]\n    },\n    \"MediaStreamOutputConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaStreamOutputConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamOutputConfigurations\"\n          },\n          \"description\": \"The configuration for each media stream that is associated with the output.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the output. This value must be unique within the current flow.\"\n        }\n      ]\n    },\n    \"OutputArn\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputArn\"\n          },\n          \"description\": \"The ARN of the output.\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The port to use when content is distributed to this output.\"\n        }\n      ]\n    },\n    \"Transport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Transport\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transport\"\n          },\n          \"description\": \"Attributes related to the transport stream that are used in the output.\"\n        }\n      ]\n    },\n    \"VpcInterfaceAttachment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcInterfaceAttachment\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaceAttachment\"\n          },\n          \"description\": \"The name of the VPC interface attachment to use for this output.\"\n        }\n      ]\n    },\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The ARN of the bridge that added this output.\"\n        }\n      ]\n    },\n    \"BridgePorts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgePorts\"\n          },\n          \"description\": \"The bridge output ports currently in use.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-output-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Output
---
