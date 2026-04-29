---
description: StartConnectionRequest schema from Amazon Outposts
layout: schema
name: StartConnectionRequest
properties_list:
- description: ''
  name: DeviceSerialNumber
  type: object
- description: ''
  name: AssetId
  type: object
- description: ''
  name: ClientPublicKey
  type: object
- description: ''
  name: NetworkInterfaceDeviceIndex
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-start-connection-request-schema.json
slug: openapi-start-connection-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-start-connection-request-schema.json\",\n  \"title\": \"StartConnectionRequest\",\n  \"description\": \"StartConnectionRequest schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceSerialNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceSerialNumber\"\n        },\n        {\n          \"description\": \" The serial number of the dongle. \"\n        }\n      ]\n    },\n    \"AssetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetId\"\n        },\n        {\n          \"description\": \" The ID of the Outpost server. \"\n        }\n      ]\n    },\n    \"ClientPublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WireGuardPublicKey\"\n        },\n\
  \        {\n          \"description\": \" The public key of the client. \"\n        }\n      ]\n    },\n    \"NetworkInterfaceDeviceIndex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaceDeviceIndex\"\n        },\n        {\n          \"description\": \" The device index of the network interface on the Outpost server. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeviceSerialNumber\",\n    \"AssetId\",\n    \"ClientPublicKey\",\n    \"NetworkInterfaceDeviceIndex\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-start-connection-request-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: StartConnectionRequest
---
