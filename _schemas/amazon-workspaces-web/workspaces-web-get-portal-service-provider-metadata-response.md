---
description: GetPortalServiceProviderMetadataResponse schema from Amazon WorkSpaces Web API
layout: schema
name: GetPortalServiceProviderMetadataResponse
properties_list:
- description: ''
  name: portalArn
  type: object
- description: ''
  name: serviceProviderSamlMetadata
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-get-portal-service-provider-metadata-response-schema.json
slug: workspaces-web-get-portal-service-provider-metadata-response
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"portalArn\"\n  ],\n  \"properties\": {\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the web portal.\"\n        }\n      ]\n    },\n    \"serviceProviderSamlMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlMetadata\"\n        },\n        {\n          \"description\": \"The service provider SAML metadata.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetPortalServiceProviderMetadataResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-portal-service-provider-metadata-response-schema.json\",\n  \"description\": \"GetPortalServiceProviderMetadataResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-portal-service-provider-metadata-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: GetPortalServiceProviderMetadataResponse
---
