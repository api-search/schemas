---
description: The container for <code>SnowconeDeviceConfiguration</code>.
layout: schema
name: DeviceConfiguration
properties_list:
- description: ''
  name: SnowconeDeviceConfiguration
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-device-configuration-schema.json
slug: amazon-snow-family-device-configuration
source_filename: amazon-snow-family-device-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-device-configuration-schema.json\",\n  \"title\": \"DeviceConfiguration\",\n  \"description\": \"The container for <code>SnowconeDeviceConfiguration</code>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnowconeDeviceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowconeDeviceConfiguration\"\n        },\n        {\n          \"description\": \"Returns information about the device configuration for an Snowcone job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-device-configuration-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DeviceConfiguration
---
