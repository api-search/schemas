---
description: Attributes related to the transport stream that are used in a source or output.
layout: schema
name: Transport
properties_list:
- description: ''
  name: CidrAllowList
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
  name: MinLatency
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
  name: SenderIpAddress
  type: object
- description: ''
  name: SmoothingLatency
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
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-transport-schema.json
slug: mediaconnect-api-transport
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-transport-schema.json\",\n  \"title\": \"Transport\",\n  \"description\": \"Attributes related to the transport stream that are used in a source or output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CidrAllowList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cidrAllowList\"\n          },\n          \"description\": \"The range of IP addresses that should be allowed to initiate output requests to this flow. These IP addresses should be in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.\"\n        }\n      ]\n    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"The smoothing max bitrate (in bps) for RIST, RTP, and RTP-FEC streams.\"\n        }\n      ]\n    },\n    \"MaxLatency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxLatency\"\n          },\n          \"description\": \"The maximum latency in milliseconds. This parameter applies only to RIST-based, Zixi-based, and Fujitsu-based streams.\"\n        }\n      ]\n    },\n    \"MaxSyncBuffer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxSyncBuffer\"\n          },\n          \"description\": \"The size of the buffer (in milliseconds) to use to sync incoming source data.\"\n        }\n      ]\n    },\n    \"MinLatency\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minLatency\"\n          },\n          \"description\": \"The minimum latency in milliseconds for SRT-based streams. In streams that use the SRT protocol, this value that you set on your MediaConnect source or output represents the minimal potential latency of that connection. The latency of the stream is set to the highest number between the sender\\u2019s minimum latency and the receiver\\u2019s minimum latency.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The protocol that is used by the source or output.\"\n        }\n      ]\n    },\n    \"RemoteId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteId\"\n          },\n          \"description\": \"The remote ID for the Zixi-pull stream.\"\n        }\n      ]\n    },\n    \"SenderControlPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"senderControlPort\"\n          },\n          \"description\": \"The port that the flow uses to send outbound requests to initiate connection with the sender.\"\n        }\n      ]\n    },\n    \"SenderIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"senderIpAddress\"\n          },\n          \"description\": \"The IP address that the flow communicates with to initiate connection with the sender.\"\n        }\n      ]\n    },\n    \"SmoothingLatency\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"smoothingLatency\"\n          },\n          \"description\": \"The smoothing latency in milliseconds for RIST, RTP, and RTP-FEC streams.\"\n        }\n      ]\n    },\n    \"SourceListenerAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceListenerAddress\"\n          },\n          \"description\": \"Source IP or domain name for SRT-caller protocol.\"\n        }\n      ]\n    },\n    \"SourceListenerPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceListenerPort\"\n          },\n          \"description\": \"Source port for SRT-caller protocol.\"\n        }\n      ]\n    },\n    \"StreamId\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamId\"\n          },\n          \"description\": \"The stream ID that you want to use for this transport. This parameter applies only to Zixi and SRT caller-based streams.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Protocol\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-transport-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Transport
---
