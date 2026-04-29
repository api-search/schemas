---
description: UpdateIpAccessSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: UpdateIpAccessSettingsResponse
properties_list:
- description: ''
  name: ipAccessSettings
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-update-ip-access-settings-response-schema.json
slug: workspaces-web-update-ip-access-settings-response
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ipAccessSettings\"\n  ],\n  \"properties\": {\n    \"ipAccessSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAccessSettings\"\n        },\n        {\n          \"description\": \"The IP access settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateIpAccessSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-ip-access-settings-response-schema.json\",\n  \"description\": \"UpdateIpAccessSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-ip-access-settings-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: UpdateIpAccessSettingsResponse
---
