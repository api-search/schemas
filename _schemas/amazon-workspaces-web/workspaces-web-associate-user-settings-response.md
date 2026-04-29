---
description: AssociateUserSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: AssociateUserSettingsResponse
properties_list:
- description: ''
  name: portalArn
  type: object
- description: ''
  name: userSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-associate-user-settings-response-schema.json
slug: workspaces-web-associate-user-settings-response
source_filename: workspaces-web-associate-user-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"portalArn\",\n    \"userSettingsArn\"\n  ],\n  \"properties\": {\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the web portal.\"\n        }\n      ]\n    },\n    \"userSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociateUserSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-user-settings-response-schema.json\",\n  \"description\": \"AssociateUserSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-user-settings-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: AssociateUserSettingsResponse
---
