---
description: UpdateNetworkSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: UpdateNetworkSettingsResponse
properties_list:
- description: ''
  name: networkSettings
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-update-network-settings-response-schema.json
slug: workspaces-web-update-network-settings-response
source_filename: workspaces-web-update-network-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"networkSettings\"\n  ],\n  \"properties\": {\n    \"networkSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkSettings\"\n        },\n        {\n          \"description\": \"The network settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateNetworkSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-network-settings-response-schema.json\",\n  \"description\": \"UpdateNetworkSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-network-settings-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: UpdateNetworkSettingsResponse
---
