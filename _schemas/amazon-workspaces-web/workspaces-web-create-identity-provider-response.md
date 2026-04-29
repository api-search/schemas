---
description: CreateIdentityProviderResponse schema from Amazon WorkSpaces Web API
layout: schema
name: CreateIdentityProviderResponse
properties_list:
- description: ''
  name: identityProviderArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-create-identity-provider-response-schema.json
slug: workspaces-web-create-identity-provider-response
source_filename: workspaces-web-create-identity-provider-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"identityProviderArn\"\n  ],\n  \"properties\": {\n    \"identityProviderArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the identity provider.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateIdentityProviderResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-identity-provider-response-schema.json\",\n  \"description\": \"CreateIdentityProviderResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-create-identity-provider-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: CreateIdentityProviderResponse
---
