---
description: The browser settings resource that can be associated with a web portal. Once associated with a web portal, browser settings control how the browser will behave once a user starts a streaming session for the web portal.
layout: schema
name: BrowserSettings
properties_list:
- description: ''
  name: associatedPortalArns
  type: object
- description: ''
  name: browserPolicy
  type: object
- description: ''
  name: browserSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-browser-settings-schema.json
slug: workspaces-web-browser-settings
source_filename: workspaces-web-browser-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"browserSettingsArn\"\n  ],\n  \"properties\": {\n    \"associatedPortalArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnList\"\n        },\n        {\n          \"description\": \"A list of web portal ARNs that this browser settings is associated with.\"\n        }\n      ]\n    },\n    \"browserPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrowserPolicy\"\n        },\n        {\n          \"description\": \"A JSON string containing Chrome Enterprise policies that will be applied to all streaming sessions.\"\n        }\n      ]\n    },\n    \"browserSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the browser settings.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The browser settings resource that can be associated with\
  \ a web portal. Once associated with a web portal, browser settings control how the browser will behave once a user starts a streaming session for the web portal. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserSettings\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-browser-settings-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-browser-settings-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: BrowserSettings
---
