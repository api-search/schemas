---
description: DescribeVTLDevicesOutput
layout: schema
name: DescribeVTLDevicesOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: VTLDevices
  type: object
- description: ''
  name: Marker
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-vtl-devices-output-schema.json
slug: amazon-storage-gateway-describe-vtl-devices-output
source_filename: amazon-storage-gateway-describe-vtl-devices-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-vtl-devices-output-schema.json\",\n  \"title\": \"DescribeVTLDevicesOutput\",\n  \"description\": \"DescribeVTLDevicesOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"VTLDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDevices\"\n        },\n        {\n          \"description\": \"An array of VTL device objects composed of the Amazon Resource Name (ARN) of the VTL devices.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"An opaque string that indicates the position at which the VTL devices that\
  \ were fetched for description ended. Use the marker in your next request to fetch the next set of VTL devices in the list. If there are no more VTL devices to describe, this field does not appear in the response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-vtl-devices-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeVTLDevicesOutput
---
