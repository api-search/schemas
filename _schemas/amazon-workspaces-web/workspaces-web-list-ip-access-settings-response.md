---
description: ListIpAccessSettingsResponse schema from Amazon WorkSpaces Web API
layout: schema
name: ListIpAccessSettingsResponse
properties_list:
- description: ''
  name: ipAccessSettings
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-list-ip-access-settings-response-schema.json
slug: workspaces-web-list-ip-access-settings-response
source_filename: workspaces-web-list-ip-access-settings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipAccessSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAccessSettingsList\"\n        },\n        {\n          \"description\": \"The IP access settings.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The pagination token used to retrieve the next page of results for this operation.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListIpAccessSettingsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-ip-access-settings-response-schema.json\",\n  \"description\": \"ListIpAccessSettingsResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-ip-access-settings-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: ListIpAccessSettingsResponse
---
