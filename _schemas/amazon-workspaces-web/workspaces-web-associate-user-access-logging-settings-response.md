---
description: AssociateUserAccessLoggingSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: AssociateUserAccessLoggingSettingsResponse
properties_list:
- description: ''
  name: portalArn
  type: object
- description: ''
  name: userAccessLoggingSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-associate-user-access-logging-settings-response-schema.json
slug: workspaces-web-associate-user-access-logging-settings-response
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"portalArn\",\n    \"userAccessLoggingSettingsArn\"\n  ],\n  \"properties\": {\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the web portal.\"\n        }\n      ]\n    },\n    \"userAccessLoggingSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user access logging settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociateUserAccessLoggingSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-user-access-logging-settings-response-schema.json\",\n  \"description\": \"AssociateUserAccessLoggingSettingsResponse schema\
  \ from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-user-access-logging-settings-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: AssociateUserAccessLoggingSettingsResponse
---
