---
description: GetTrustStoreResponse schema from Amazon WorkSpaces Web API
layout: schema
name: GetTrustStoreResponse
properties_list:
- description: ''
  name: trustStore
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-get-trust-store-response-schema.json
slug: workspaces-web-get-trust-store-response
source_filename: workspaces-web-get-trust-store-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"trustStore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustStore\"\n        },\n        {\n          \"description\": \"The trust store.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetTrustStoreResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-trust-store-response-schema.json\",\n  \"description\": \"GetTrustStoreResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-trust-store-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: GetTrustStoreResponse
---
