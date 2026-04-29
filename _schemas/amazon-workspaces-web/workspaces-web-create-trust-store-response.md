---
description: CreateTrustStoreResponse schema from Amazon WorkSpaces Web API
layout: schema
name: CreateTrustStoreResponse
properties_list:
- description: ''
  name: trustStoreArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-create-trust-store-response-schema.json
slug: workspaces-web-create-trust-store-response
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"trustStoreArn\"\n  ],\n  \"properties\": {\n    \"trustStoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the trust store.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTrustStoreResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-trust-store-response-schema.json\",\n  \"description\": \"CreateTrustStoreResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-trust-store-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: CreateTrustStoreResponse
---
