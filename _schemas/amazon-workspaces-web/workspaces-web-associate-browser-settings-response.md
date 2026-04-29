---
description: AssociateBrowserSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: AssociateBrowserSettingsResponse
properties_list:
- description: ''
  name: browserSettingsArn
  type: object
- description: ''
  name: portalArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-associate-browser-settings-response-schema.json
slug: workspaces-web-associate-browser-settings-response
source_filename: workspaces-web-associate-browser-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"browserSettingsArn\",\n    \"portalArn\"\n  ],\n  \"properties\": {\n    \"browserSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the browser settings.\"\n        }\n      ]\n    },\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the web portal.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociateBrowserSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-browser-settings-response-schema.json\",\n  \"description\": \"AssociateBrowserSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-browser-settings-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: AssociateBrowserSettingsResponse
---
