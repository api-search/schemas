---
description: The summary of the trust store.
layout: schema
name: TrustStoreSummary
properties_list:
- description: ''
  name: trustStoreArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-trust-store-summary-schema.json
slug: workspaces-web-trust-store-summary
source_filename: workspaces-web-trust-store-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"trustStoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the trust store.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The summary of the trust store.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TrustStoreSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-trust-store-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-trust-store-summary-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: TrustStoreSummary
---
