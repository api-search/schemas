---
description: DescribeVTLDevicesInput
layout: schema
name: DescribeVTLDevicesInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: VTLDeviceARNs
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-vtl-devices-input-schema.json
slug: amazon-storage-gateway-describe-vtl-devices-input
source_filename: amazon-storage-gateway-describe-vtl-devices-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-vtl-devices-input-schema.json\",\n  \"title\": \"DescribeVTLDevicesInput\",\n  \"description\": \"DescribeVTLDevicesInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"VTLDeviceARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDeviceARNs\"\n        },\n        {\n          \"description\": \"<p>An array of strings, where each string represents the Amazon Resource Name (ARN) of a VTL device.</p> <note> <p>All of the specified VTL devices must be from the same gateway. If no VTL devices are specified, the result will contain all devices on the specified gateway.</p> </note>\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"An opaque string that indicates the position at which to begin describing the VTL devices.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"Specifies that the number of VTL devices described be limited to the specified number.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-vtl-devices-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeVTLDevicesInput
---
