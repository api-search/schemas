---
description: UpdateBrowserSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: UpdateBrowserSettingsResponse
properties_list:
- description: ''
  name: browserSettings
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-update-browser-settings-response-schema.json
slug: workspaces-web-update-browser-settings-response
source_filename: workspaces-web-update-browser-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"browserSettings\"\n  ],\n  \"properties\": {\n    \"browserSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrowserSettings\"\n        },\n        {\n          \"description\": \"The browser settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateBrowserSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-browser-settings-response-schema.json\",\n  \"description\": \"UpdateBrowserSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-browser-settings-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: UpdateBrowserSettingsResponse
---
