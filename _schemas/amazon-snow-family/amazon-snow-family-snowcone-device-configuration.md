---
description: Specifies the device configuration for an Snowcone job.
layout: schema
name: SnowconeDeviceConfiguration
properties_list:
- description: ''
  name: WirelessConnection
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-snowcone-device-configuration-schema.json
slug: amazon-snow-family-snowcone-device-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-snowcone-device-configuration-schema.json\",\n  \"title\": \"SnowconeDeviceConfiguration\",\n  \"description\": \"Specifies the device configuration for an Snowcone job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WirelessConnection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WirelessConnection\"\n        },\n        {\n          \"description\": \"Configures the wireless connection for the Snowcone device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-snowcone-device-configuration-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: SnowconeDeviceConfiguration
---
