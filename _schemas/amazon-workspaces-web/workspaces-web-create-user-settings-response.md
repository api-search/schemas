---
description: CreateUserSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: CreateUserSettingsResponse
properties_list:
- description: ''
  name: userSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-create-user-settings-response-schema.json
slug: workspaces-web-create-user-settings-response
source_filename: workspaces-web-create-user-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"userSettingsArn\"\n  ],\n  \"properties\": {\n    \"userSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateUserSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-user-settings-response-schema.json\",\n  \"description\": \"CreateUserSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-user-settings-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: CreateUserSettingsResponse
---
