---
description: DescribeDeviceResponse schema from Amazon Panorama
layout: schema
name: DescribeDeviceResponse
properties_list:
- description: ''
  name: AlternateSoftwares
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Brand
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: CurrentNetworkingStatus
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
  name: DeviceConnectionStatus
  type: object
- description: ''
  name: DeviceId
  type: object
- description: ''
  name: LatestAlternateSoftware
  type: object
- description: ''
  name: LatestDeviceJob
  type: object
- description: ''
  name: LatestSoftware
  type: object
- description: ''
  name: LeaseExpirationTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: NetworkingConfiguration
  type: object
- description: ''
  name: ProvisioningStatus
  type: object
- description: ''
  name: SerialNumber
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-device-response-schema.json
slug: openapi-describe-device-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-device-response-schema.json\",\n  \"title\": \"DescribeDeviceResponse\",\n  \"description\": \"DescribeDeviceResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlternateSoftwares\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlternateSoftwares\"\n        },\n        {\n          \"description\": \"Beta software releases available for the device.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceArn\"\n        },\n        {\n          \"description\": \"The device's ARN.\"\n        }\n      ]\n    },\n    \"Brand\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceBrand\"\n        },\n        {\n      \
  \    \"description\": \"The device's maker.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTime\"\n        },\n        {\n          \"description\": \"When the device was created.\"\n        }\n      ]\n    },\n    \"CurrentNetworkingStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkStatus\"\n        },\n        {\n          \"description\": \"The device's networking status.\"\n        }\n      ]\n    },\n    \"CurrentSoftware\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentSoftware\"\n        },\n        {\n          \"description\": \"The device's current software version.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The device's description.\"\n        }\n      ]\n\
  \    },\n    \"DeviceAggregatedStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceAggregatedStatus\"\n        },\n        {\n          \"description\": \"A device's aggregated status. Including the device's connection status, provisioning status, and lease status.\"\n        }\n      ]\n    },\n    \"DeviceConnectionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceConnectionStatus\"\n        },\n        {\n          \"description\": \"The device's connection status.\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"The device's ID.\"\n        }\n      ]\n    },\n    \"LatestAlternateSoftware\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatestAlternateSoftware\"\n        },\n        {\n          \"description\": \"The most recent\
  \ beta software release.\"\n        }\n      ]\n    },\n    \"LatestDeviceJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatestDeviceJob\"\n        },\n        {\n          \"description\": \"A device's latest job. Includes the target image version, and the job status.\"\n        }\n      ]\n    },\n    \"LatestSoftware\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatestSoftware\"\n        },\n        {\n          \"description\": \"The latest software version available for the device.\"\n        }\n      ]\n    },\n    \"LeaseExpirationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LeaseExpirationTime\"\n        },\n        {\n          \"description\": \"The device's lease expiration time.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceName\"\n        },\n        {\n          \"description\": \"\
  The device's name.\"\n        }\n      ]\n    },\n    \"NetworkingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkPayload\"\n        },\n        {\n          \"description\": \"The device's networking configuration.\"\n        }\n      ]\n    },\n    \"ProvisioningStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceStatus\"\n        },\n        {\n          \"description\": \"The device's provisioning status.\"\n        }\n      ]\n    },\n    \"SerialNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceSerialNumber\"\n        },\n        {\n          \"description\": \"The device's serial number.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The device's tags.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"The device's type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-device-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribeDeviceResponse
---
