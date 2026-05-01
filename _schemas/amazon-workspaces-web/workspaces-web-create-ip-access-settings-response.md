---
description: CreateIpAccessSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: CreateIpAccessSettingsResponse
properties_list:
- description: ''
  name: ipAccessSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-create-ip-access-settings-response-schema.json
slug: workspaces-web-create-ip-access-settings-response
source_filename: workspaces-web-create-ip-access-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ipAccessSettingsArn\"\n  ],\n  \"properties\": {\n    \"ipAccessSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the IP access settings resource.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateIpAccessSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-ip-access-settings-response-schema.json\",\n  \"description\": \"CreateIpAccessSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-ip-access-settings-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: CreateIpAccessSettingsResponse
---
