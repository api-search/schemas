---
description: GetIdentityProviderResponse schema from Amazon WorkSpaces Web API
layout: schema
name: GetIdentityProviderResponse
properties_list:
- description: ''
  name: identityProvider
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-get-identity-provider-response-schema.json
slug: workspaces-web-get-identity-provider-response
source_filename: workspaces-web-get-identity-provider-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"identityProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProvider\"\n        },\n        {\n          \"description\": \"The identity provider.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetIdentityProviderResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-identity-provider-response-schema.json\",\n  \"description\": \"GetIdentityProviderResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-identity-provider-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: GetIdentityProviderResponse
---
