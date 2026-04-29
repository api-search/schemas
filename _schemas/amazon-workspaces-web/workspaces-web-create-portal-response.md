---
description: CreatePortalResponse schema from Amazon WorkSpaces Web API
layout: schema
name: CreatePortalResponse
properties_list:
- description: ''
  name: portalArn
  type: object
- description: ''
  name: portalEndpoint
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-create-portal-response-schema.json
slug: workspaces-web-create-portal-response
source_filename: workspaces-web-create-portal-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"portalArn\",\n    \"portalEndpoint\"\n  ],\n  \"properties\": {\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the web portal.\"\n        }\n      ]\n    },\n    \"portalEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalEndpoint\"\n        },\n        {\n          \"description\": \"The endpoint URL of the web portal that users access in order to start streaming sessions.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreatePortalResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-portal-response-schema.json\",\n  \"description\": \"CreatePortalResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-portal-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: CreatePortalResponse
---
