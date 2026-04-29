---
description: ProvisionDeviceRequest schema from Amazon Panorama
layout: schema
name: ProvisionDeviceRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: NetworkingConfiguration
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-provision-device-request-schema.json
slug: openapi-provision-device-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-provision-device-request-schema.json\",\n  \"title\": \"ProvisionDeviceRequest\",\n  \"description\": \"ProvisionDeviceRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description for the device.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceName\"\n        },\n        {\n          \"description\": \"A name for the device.\"\n        }\n      ]\n    },\n    \"NetworkingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkPayload\"\n        },\n        {\n          \"\
  description\": \"A networking configuration for the device.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-provision-device-request-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ProvisionDeviceRequest
---
