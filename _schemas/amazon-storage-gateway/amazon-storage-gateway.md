---
description: Schema representing an AWS Storage Gateway resource. A Storage Gateway connects on-premises environments to AWS cloud storage, enabling hybrid cloud storage workflows with local caching for low-latency access.
layout: schema
name: Amazon Storage Gateway
properties_list:
- description: The Amazon Resource Name (ARN) of the gateway.
  name: GatewayARN
  type: string
- description: The unique identifier assigned to the gateway.
  name: GatewayId
  type: string
- description: The name of the gateway.
  name: GatewayName
  type: string
- description: A value that indicates the time zone configured for the gateway.
  name: GatewayTimezone
  type: string
- description: The type of the gateway.
  name: GatewayType
  type: string
- description: A value that indicates the operating state of the gateway.
  name: GatewayState
  type: string
- description: The state of the gateway.
  name: GatewayOperationalState
  type: string
- description: The ID of the Amazon EC2 instance that was used to launch the gateway.
  name: Ec2InstanceId
  type: string
- description: The AWS Region where the Amazon EC2 instance is located.
  name: Ec2InstanceRegion
  type: string
- description: A list of network interfaces on the gateway.
  name: GatewayNetworkInterfaces
  type: array
- description: The date on which the last software update was applied to the gateway.
  name: LastSoftwareUpdate
  type: string
- description: The date on which an update to the gateway is available.
  name: NextUpdateAvailabilityDate
  type: string
- description: A list of tags assigned to the gateway.
  name: Tags
  type: array
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-schema.json
slug: amazon-storage-gateway
source_filename: amazon-storage-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://schema.api.io/amazon-storage-gateway/amazon-storage-gateway-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Amazon Storage Gateway\",\n  \"description\": \"Schema representing an AWS Storage Gateway resource. A Storage Gateway connects on-premises environments to AWS cloud storage, enabling hybrid cloud storage workflows with local caching for low-latency access.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"GatewayARN\"\n  ],\n  \"properties\": {\n    \"GatewayARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the gateway.\",\n      \"pattern\": \"^arn:aws:storagegateway:[a-z0-9-]+:[0-9]{12}:gateway/sgw-[A-F0-9]+$\"\n    },\n    \"GatewayId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the gateway.\",\n      \"pattern\": \"^sgw-[A-F0-9]+$\"\n    },\n    \"GatewayName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The name of the gateway.\",\n      \"minLength\": 2,\n      \"maxLength\": 255\n    },\n    \"GatewayTimezone\": {\n      \"type\": \"string\",\n      \"description\": \"A value that indicates the time zone configured for the gateway.\",\n      \"examples\": [\"GMT-5:00\", \"GMT\", \"GMT+1:00\"]\n    },\n    \"GatewayType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the gateway.\",\n      \"enum\": [\"STORED\", \"CACHED\", \"VTL\", \"S3_FILE_GATEWAY\", \"FSX_SMB\"]\n    },\n    \"GatewayState\": {\n      \"type\": \"string\",\n      \"description\": \"A value that indicates the operating state of the gateway.\",\n      \"enum\": [\"RUNNING\", \"SHUTDOWN\"]\n    },\n    \"GatewayOperationalState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the gateway.\",\n      \"enum\": [\"ACTIVE\", \"SHUTDOWN\"]\n    },\n    \"Ec2InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Amazon\
  \ EC2 instance that was used to launch the gateway.\"\n    },\n    \"Ec2InstanceRegion\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS Region where the Amazon EC2 instance is located.\"\n    },\n    \"GatewayNetworkInterfaces\": {\n      \"type\": \"array\",\n      \"description\": \"A list of network interfaces on the gateway.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/NetworkInterface\"\n      }\n    },\n    \"LastSoftwareUpdate\": {\n      \"type\": \"string\",\n      \"description\": \"The date on which the last software update was applied to the gateway.\"\n    },\n    \"NextUpdateAvailabilityDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date on which an update to the gateway is available.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tags assigned to the gateway.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"NetworkInterface\":\
  \ {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Ipv4Address\": {\n          \"type\": \"string\",\n          \"description\": \"The Internet Protocol version 4 (IPv4) address of the interface.\",\n          \"format\": \"ipv4\"\n        },\n        \"MacAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The Media Access Control (MAC) address of the interface.\"\n        },\n        \"Ipv6Address\": {\n          \"type\": \"string\",\n          \"description\": \"The Internet Protocol version 6 (IPv6) address of the interface.\",\n          \"format\": \"ipv6\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\"Key\", \"Value\"],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"description\": \"Tag key.\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Tag value.\",\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: Amazon Storage Gateway
---
