---
description: AssociateTrustStoreResponse schema from Amazon WorkSpaces Web API
layout: schema
name: AssociateTrustStoreResponse
properties_list:
- description: ''
  name: portalArn
  type: object
- description: ''
  name: trustStoreArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-associate-trust-store-response-schema.json
slug: workspaces-web-associate-trust-store-response
source_filename: workspaces-web-associate-trust-store-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"portalArn\",\n    \"trustStoreArn\"\n  ],\n  \"properties\": {\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the web portal.\"\n        }\n      ]\n    },\n    \"trustStoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the trust store.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociateTrustStoreResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-trust-store-response-schema.json\",\n  \"description\": \"AssociateTrustStoreResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-associate-trust-store-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: AssociateTrustStoreResponse
---
