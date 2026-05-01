---
description: ListUserAccessLoggingSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: ListUserAccessLoggingSettingsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: userAccessLoggingSettings
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-list-user-access-logging-settings-response-schema.json
slug: workspaces-web-list-user-access-logging-settings-response
source_filename: workspaces-web-list-user-access-logging-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The pagination token used to retrieve the next page of results for this operation.\"\n        }\n      ]\n    },\n    \"userAccessLoggingSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserAccessLoggingSettingsList\"\n        },\n        {\n          \"description\": \"The user access logging settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListUserAccessLoggingSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-user-access-logging-settings-response-schema.json\",\n  \"description\": \"ListUserAccessLoggingSettingsResponse schema from Amazon WorkSpaces\
  \ Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-user-access-logging-settings-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: ListUserAccessLoggingSettingsResponse
---
