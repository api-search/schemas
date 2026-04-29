---
description: The summary of the identity provider.
layout: schema
name: IdentityProviderSummary
properties_list:
- description: ''
  name: identityProviderArn
  type: object
- description: ''
  name: identityProviderName
  type: object
- description: ''
  name: identityProviderType
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-identity-provider-summary-schema.json
slug: workspaces-web-identity-provider-summary
source_filename: workspaces-web-identity-provider-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"identityProviderArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the identity provider.\"\n        }\n      ]\n    },\n    \"identityProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderName\"\n        },\n        {\n          \"description\": \"The identity provider name.\"\n        }\n      ]\n    },\n    \"identityProviderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderType\"\n        },\n        {\n          \"description\": \"The identity provider type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The summary of the identity provider.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IdentityProviderSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-identity-provider-summary-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-identity-provider-summary-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: IdentityProviderSummary
---
