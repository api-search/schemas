---
description: Configures the wireless connection on an Snowcone device.
layout: schema
name: WirelessConnection
properties_list:
- description: ''
  name: IsWifiEnabled
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-wireless-connection-schema.json
slug: amazon-snow-family-wireless-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-wireless-connection-schema.json\",\n  \"title\": \"WirelessConnection\",\n  \"description\": \"Configures the wireless connection on an Snowcone device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IsWifiEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Enables the Wi-Fi adapter on an Snowcone device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-wireless-connection-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: WirelessConnection
---
