---
description: GetUserAccessLoggingSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: GetUserAccessLoggingSettingsResponse
properties_list:
- description: ''
  name: userAccessLoggingSettings
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-get-user-access-logging-settings-response-schema.json
slug: workspaces-web-get-user-access-logging-settings-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"userAccessLoggingSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserAccessLoggingSettings\"\n        },\n        {\n          \"description\": \"The user access logging settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetUserAccessLoggingSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-user-access-logging-settings-response-schema.json\",\n  \"description\": \"GetUserAccessLoggingSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-user-access-logging-settings-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: GetUserAccessLoggingSettingsResponse
---
