---
description: GetNetworkSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: GetNetworkSettingsResponse
properties_list:
- description: ''
  name: networkSettings
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-get-network-settings-response-schema.json
slug: workspaces-web-get-network-settings-response
source_filename: workspaces-web-get-network-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkSettings\"\n        },\n        {\n          \"description\": \"The network settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetNetworkSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-network-settings-response-schema.json\",\n  \"description\": \"GetNetworkSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-network-settings-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: GetNetworkSettingsResponse
---
