---
description: The settings for the source of the flow.
layout: schema
name: Source
properties_list:
- description: ''
  name: DataTransferSubscriberFeePercent
  type: object
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
  name: IngestIp
  type: object
- description: ''
  name: IngestPort
  type: object
- description: ''
  name: MediaStreamSourceConfigurations
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: SenderControlPort
  type: object
- description: ''
  name: SenderIpAddress
  type: object
- description: ''
  name: SourceArn
  type: object
- description: ''
  name: Transport
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
schema_file: json-schema/mediaconnect-api-source-schema.json
slug: mediaconnect-api-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-source-schema.json\",\n  \"title\": \"Source\",\n  \"description\": \"The settings for the source of the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataTransferSubscriberFeePercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataTransferSubscriberFeePercent\"\n          },\n          \"description\": \"Percentage from 0-100 of the data transfer cost to be billed to the subscriber.\"\n        }\n      ]\n    },\n    \"Decryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"decryption\"\n          },\n          \"description\": \"The\
  \ type of encryption that is used on the content ingested from this source.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A description for the source. This value is not used or seen outside of the current AWS Elemental MediaConnect account.\"\n        }\n      ]\n    },\n    \"EntitlementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlementArn\"\n          },\n          \"description\": \"The ARN of the entitlement that allows you to subscribe to content that comes from another AWS account. The entitlement is set by the content originator and the ARN is generated as part of the originator's flow.\"\n        }\n      ]\n    },\n    \"IngestIp\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingestIp\"\n          },\n          \"description\": \"The IP address that the flow will be listening on for incoming content.\"\n        }\n      ]\n    },\n    \"IngestPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingestPort\"\n          },\n          \"description\": \"The port that the flow will be listening on for incoming content.\"\n        }\n      ]\n    },\n    \"MediaStreamSourceConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaStreamSourceConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreamSourceConfigurations\"\n          },\n          \"description\": \"The media streams that are associated with the\
  \ source, and the parameters for those associations.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the source.\"\n        }\n      ]\n    },\n    \"SenderControlPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"senderControlPort\"\n          },\n          \"description\": \"The port that the flow uses to send outbound requests to initiate connection with the sender.\"\n        }\n      ]\n    },\n    \"SenderIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"senderIpAddress\"\n          },\n          \"description\": \"The IP address that\
  \ the flow communicates with to initiate connection with the sender.\"\n        }\n      ]\n    },\n    \"SourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceArn\"\n          },\n          \"description\": \"The ARN of the source.\"\n        }\n      ]\n    },\n    \"Transport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Transport\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transport\"\n          },\n          \"description\": \"Attributes related to the transport stream that are used in the source.\"\n        }\n      ]\n    },\n    \"VpcInterfaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaceName\"\n          },\n          \"description\": \"The name of the VPC interface\
  \ that is used for this source.\"\n        }\n      ]\n    },\n    \"WhitelistCidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"whitelistCidr\"\n          },\n          \"description\": \"The range of IP addresses that should be allowed to contribute content to your source. These IP addresses should be in the form of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.\"\n        }\n      ]\n    },\n    \"GatewayBridgeSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayBridgeSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gatewayBridgeSource\"\n          },\n          \"description\": \"The source configuration for cloud flows receiving a stream from a bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"SourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-source-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Source
---
