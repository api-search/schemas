---
description: The settings for the source of the flow.
layout: schema
name: SetSourceRequest
properties_list:
- description: ''
  name: Decryption
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EntitlementArn
  type: object
- description: ''
  name: IngestPort
  type: object
- description: ''
  name: MaxBitrate
  type: object
- description: ''
  name: MaxLatency
  type: object
- description: ''
  name: MaxSyncBuffer
  type: object
- description: ''
  name: MediaStreamSourceConfigurations
  type: object
- description: ''
  name: MinLatency
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Protocol
  type: object
- description: ''
  name: SenderControlPort
  type: object
- description: ''
  name: SenderIpAddress
  type: object
- description: ''
  name: SourceListenerAddress
  type: object
- description: ''
  name: SourceListenerPort
  type: object
- description: ''
  name: StreamId
  type: object
- description: ''
  name: VpcInterfaceName
  type: object
- description: ''
  name: WhitelistCidr
  type: object
- description: ''
  name: GatewayBridgeSource
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-set-source-request-schema.json
slug: mediaconnect-api-set-source-request
source_filename: mediaconnect-api-set-source-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-set-source-request-schema.json\",\n  \"title\": \"SetSourceRequest\",\n  \"description\": \"The settings for the source of the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Decryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"decryption\"\n          },\n          \"description\": \"The type of encryption that is used on the content ingested from this source. Allowable encryption types: static-key.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\"\
  : \"A description for the source. This value is not used or seen outside of the current AWS Elemental MediaConnect account.\"\n        }\n      ]\n    },\n    \"EntitlementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"pattern\": \"^arn:.+:mediaconnect.+:entitlement:.+$\",\n          \"xml\": {\n            \"name\": \"entitlementArn\"\n          },\n          \"description\": \"The ARN of the entitlement that allows you to subscribe to this flow. The entitlement is set by the flow originator, and the ARN is generated as part of the originator's flow.\"\n        }\n      ]\n    },\n    \"IngestPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingestPort\"\n          },\n          \"description\": \"The port that the flow will be listening on for incoming content.\"\n        }\n      ]\n \
  \   },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"The smoothing max bitrate (in bps) for RIST, RTP, and RTP-FEC streams.\"\n        }\n      ]\n    },\n    \"MaxLatency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxLatency\"\n          },\n          \"description\": \"The maximum latency in milliseconds. This parameter applies only to RIST-based, Zixi-based, and Fujitsu-based streams.\"\n        }\n      ]\n    },\n    \"MaxSyncBuffer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxSyncBuffer\"\n          },\n          \"description\": \"The size of the buffer (in\
  \ milliseconds) to use to sync incoming source data.\"\n        }\n      ]\n    },\n    \"MediaStreamSourceConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaStreamSourceConfigurationRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamSourceConfigurations\"\n          },\n          \"description\": \"The media streams that are associated with the source, and the parameters for those associations.\"\n        }\n      ]\n    },\n    \"MinLatency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minLatency\"\n          },\n          \"description\": \"The minimum latency in milliseconds for SRT-based streams. In streams that use the SRT protocol, this value that you set on your MediaConnect source or output represents the minimal potential latency of that connection. The latency of the\
  \ stream is set to the highest number between the sender\\u2019s minimum latency and the receiver\\u2019s minimum latency.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the source.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The protocol that is used by the source.\"\n        }\n      ]\n    },\n    \"SenderControlPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"senderControlPort\"\n          },\n          \"description\": \"The port that the\
  \ flow uses to send outbound requests to initiate connection with the sender.\"\n        }\n      ]\n    },\n    \"SenderIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"senderIpAddress\"\n          },\n          \"description\": \"The IP address that the flow communicates with to initiate connection with the sender.\"\n        }\n      ]\n    },\n    \"SourceListenerAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceListenerAddress\"\n          },\n          \"description\": \"Source IP or domain name for SRT-caller protocol.\"\n        }\n      ]\n    },\n    \"SourceListenerPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceListenerPort\"\
  \n          },\n          \"description\": \"Source port for SRT-caller protocol.\"\n        }\n      ]\n    },\n    \"StreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamId\"\n          },\n          \"description\": \"The stream ID that you want to use for this transport. This parameter applies only to Zixi and SRT caller-based streams.\"\n        }\n      ]\n    },\n    \"VpcInterfaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaceName\"\n          },\n          \"description\": \"The name of the VPC interface to use for this source.\"\n        }\n      ]\n    },\n    \"WhitelistCidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"whitelistCidr\"\n          },\n          \"description\": \"The range of IP addresses that should be allowed to contribute content to your source. These IP addresses should be in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.\"\n        }\n      ]\n    },\n    \"GatewayBridgeSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetGatewayBridgeSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayBridgeSource\"\n          },\n          \"description\": \"The source configuration for cloud flows receiving a stream from a bridge.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-set-source-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: SetSourceRequest
---
