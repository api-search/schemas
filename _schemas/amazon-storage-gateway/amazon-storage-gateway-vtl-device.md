---
description: Represents a device object associated with a tape gateway.
layout: schema
name: VTLDevice
properties_list:
- description: ''
  name: VTLDeviceARN
  type: object
- description: ''
  name: VTLDeviceType
  type: object
- description: ''
  name: VTLDeviceVendor
  type: object
- description: ''
  name: VTLDeviceProductIdentifier
  type: object
- description: ''
  name: DeviceiSCSIAttributes
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-vtl-device-schema.json
slug: amazon-storage-gateway-vtl-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-vtl-device-schema.json\",\n  \"title\": \"VTLDevice\",\n  \"description\": \"Represents a device object associated with a tape gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VTLDeviceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDeviceARN\"\n        },\n        {\n          \"description\": \"Specifies the unique Amazon Resource Name (ARN) of the device (tape drive or media changer).\"\n        }\n      ]\n    },\n    \"VTLDeviceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDeviceType\"\n        },\n        {\n          \"description\": \"Specifies the type of device that the VTL device emulates.\"\n        }\n      ]\n    },\n    \"VTLDeviceVendor\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/VTLDeviceVendor\"\n        },\n        {\n          \"description\": \"Specifies the vendor of the device that the VTL device object emulates.\"\n        }\n      ]\n    },\n    \"VTLDeviceProductIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDeviceProductIdentifier\"\n        },\n        {\n          \"description\": \"Specifies the model number of device that the VTL device emulates.\"\n        }\n      ]\n    },\n    \"DeviceiSCSIAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceiSCSIAttributes\"\n        },\n        {\n          \"description\": \"A list of iSCSI information about a VTL device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-vtl-device-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: VTLDevice
---
