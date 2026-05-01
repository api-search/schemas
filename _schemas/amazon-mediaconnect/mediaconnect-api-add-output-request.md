---
description: The output that you want to add to this flow.
layout: schema
name: AddOutputRequest
properties_list:
- description: ''
  name: CidrAllowList
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
  name: MaxLatency
  type: object
- description: ''
  name: MediaStreamOutputConfigurations
  type: object
- description: ''
  name: MinLatency
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: Protocol
  type: object
- description: ''
  name: RemoteId
  type: object
- description: ''
  name: SenderControlPort
  type: object
- description: ''
  name: SmoothingLatency
  type: object
- description: ''
  name: StreamId
  type: object
- description: ''
  name: VpcInterfaceAttachment
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-output-request-schema.json
slug: mediaconnect-api-add-output-request
source_filename: mediaconnect-api-add-output-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-output-request-schema.json\",\n  \"title\": \"AddOutputRequest\",\n  \"description\": \"The output that you want to add to this flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CidrAllowList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cidrAllowList\"\n          },\n          \"description\": \"The range of IP addresses that should be allowed to initiate output requests to this flow. These IP addresses should be in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n     \
  \   },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A description of the output. This description appears only on the AWS Elemental MediaConnect console and will not be seen by the end user.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"The IP address from which video will be sent to output destinations.\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          },\n          \"description\": \"The type of key used for the encryption. If no keyType is provided, the service will use the default setting (static-key). Allowable\
  \ encryption types: static-key.\"\n        }\n      ]\n    },\n    \"MaxLatency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxLatency\"\n          },\n          \"description\": \"The maximum latency in milliseconds. This parameter applies only to RIST-based, Zixi-based, and Fujitsu-based streams.\"\n        }\n      ]\n    },\n    \"MediaStreamOutputConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaStreamOutputConfigurationRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamOutputConfigurations\"\n          },\n          \"description\": \"The media streams that are associated with the output, and the parameters for those associations.\"\n        }\n      ]\n    },\n    \"MinLatency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"minLatency\"\n          },\n          \"description\": \"The minimum latency in milliseconds for SRT-based streams. In streams that use the SRT protocol, this value that you set on your MediaConnect source or output represents the minimal potential latency of that connection. The latency of the stream is set to the highest number between the sender\\u2019s minimum latency and the receiver\\u2019s minimum latency.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the output. This value must be unique within the current flow.\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n  \
  \          \"name\": \"port\"\n          },\n          \"description\": \"The port to use when content is distributed to this output.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The protocol to use for the output.\"\n        }\n      ]\n    },\n    \"RemoteId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteId\"\n          },\n          \"description\": \"The remote ID for the Zixi-pull output stream.\"\n        }\n      ]\n    },\n    \"SenderControlPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"senderControlPort\"\n          },\n      \
  \    \"description\": \"The port that the flow uses to send outbound requests to initiate connection with the sender.\"\n        }\n      ]\n    },\n    \"SmoothingLatency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"smoothingLatency\"\n          },\n          \"description\": \"The smoothing latency in milliseconds for RIST, RTP, and RTP-FEC streams.\"\n        }\n      ]\n    },\n    \"StreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamId\"\n          },\n          \"description\": \"The stream ID that you want to use for this transport. This parameter applies only to Zixi and SRT caller-based streams.\"\n        }\n      ]\n    },\n    \"VpcInterfaceAttachment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcInterfaceAttachment\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaceAttachment\"\n          },\n          \"description\": \"The name of the VPC interface attachment to use for this output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Protocol\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-output-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddOutputRequest
---
