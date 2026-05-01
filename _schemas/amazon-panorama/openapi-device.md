---
description: A device.
layout: schema
name: Device
properties_list:
- description: ''
  name: Brand
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: CurrentSoftware
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: DeviceAggregatedStatus
  type: object
- description: ''
  name: DeviceId
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: LatestDeviceJob
  type: object
- description: ''
  name: LeaseExpirationTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: ProvisioningStatus
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-device-schema.json
slug: openapi-device
source_filename: openapi-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"A device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Brand\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceBrand\"\n        },\n        {\n          \"description\": \"The device's maker.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTime\"\n        },\n        {\n          \"description\": \"When the device was created.\"\n        }\n      ]\n    },\n    \"CurrentSoftware\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentSoftware\"\n        },\n        {\n          \"description\": \"A device's current software.\"\n        }\n      ]\n    },\n    \"\
  Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description for the device.\"\n        }\n      ]\n    },\n    \"DeviceAggregatedStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceAggregatedStatus\"\n        },\n        {\n          \"description\": \"A device's aggregated status. Including the device's connection status, provisioning status, and lease status.\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"The device's ID.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTime\"\n        },\n        {\n          \"description\": \"When the device was updated.\"\n        }\n      ]\n    },\n    \"LatestDeviceJob\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatestDeviceJob\"\n        },\n        {\n          \"description\": \"A device's latest job. Includes the target image version, and the update job status.\"\n        }\n      ]\n    },\n    \"LeaseExpirationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LeaseExpirationTime\"\n        },\n        {\n          \"description\": \"The device's lease expiration time.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceName\"\n        },\n        {\n          \"description\": \"The device's name.\"\n        }\n      ]\n    },\n    \"ProvisioningStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceStatus\"\n        },\n        {\n          \"description\": \"The device's provisioning status.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The device's tags.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"The device's type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-device-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: Device
---
