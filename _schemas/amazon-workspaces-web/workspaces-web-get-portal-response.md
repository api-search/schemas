---
description: GetPortalResponse schema from Amazon WorkSpaces Web API
layout: schema
name: GetPortalResponse
properties_list:
- description: ''
  name: portal
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-get-portal-response-schema.json
slug: workspaces-web-get-portal-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"portal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Portal\"\n        },\n        {\n          \"description\": \"The web portal.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetPortalResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-portal-response-schema.json\",\n  \"description\": \"GetPortalResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-portal-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: GetPortalResponse
---
