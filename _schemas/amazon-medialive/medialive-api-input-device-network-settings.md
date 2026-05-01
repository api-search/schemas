---
description: The network settings for the input device.
layout: schema
name: InputDeviceNetworkSettings
properties_list:
- description: ''
  name: DnsAddresses
  type: object
- description: ''
  name: Gateway
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: IpScheme
  type: object
- description: ''
  name: SubnetMask
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-device-network-settings-schema.json
slug: medialive-api-input-device-network-settings
source_filename: medialive-api-input-device-network-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-network-settings-schema.json\",\n  \"title\": \"InputDeviceNetworkSettings\",\n  \"description\": \"The network settings for the input device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DnsAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dnsAddresses\"\n          },\n          \"description\": \"The DNS addresses of the input device.\"\n        }\n      ]\n    },\n    \"Gateway\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gateway\"\n          },\n          \"description\": \"The network gateway IP address.\"\n        }\n\
  \      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipAddress\"\n          },\n          \"description\": \"The IP address of the input device.\"\n        }\n      ]\n    },\n    \"IpScheme\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceIpScheme\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipScheme\"\n          },\n          \"description\": \"Specifies whether the input device has been configured (outside of MediaLive) to use a dynamic IP address assignment (DHCP) or a static IP address.\"\n        }\n      ]\n    },\n    \"SubnetMask\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetMask\"\n          },\n          \"description\": \"The subnet mask of the input\
  \ device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-network-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputDeviceNetworkSettings
---
