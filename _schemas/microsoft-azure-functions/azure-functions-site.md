---
description: A web app, a mobile app backend, or an API app.
layout: schema
name: Site
properties_list:
- description: Site resource specific properties
  name: properties
  type: object
- description: Managed service identity.
  name: identity
  type: object
- description: Extended Location.
  name: extendedLocation
  type: object
- description: Kind of resource. If the resource is an app, you can refer to https://github.com/Azure/app-service-linux-docs/blob/master/Things_You_Should_Know/kind_property.md#app-service-resource-kind-reference fo
  name: kind
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-site-schema.json
slug: azure-functions-site
source_filename: azure-functions-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-schema.json\",\n  \"title\": \"Site\",\n  \"description\": \"A web app, a mobile app backend, or an API app.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/SiteProperties\",\n      \"description\": \"Site resource specific properties\",\n      \"x-ms-client-flatten\": true\n    },\n    \"identity\": {\n      \"$ref\": \"#/definitions/ManagedServiceIdentity\",\n      \"description\": \"Managed service identity.\"\n    },\n    \"extendedLocation\": {\n      \"$ref\": \"#/definitions/ExtendedLocation\",\n      \"description\": \"Extended Location.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of resource. If the resource is an app, you can refer to https://github.com/Azure/app-service-linux-docs/blob/master/Things_You_Should_Know/kind_property.md#app-service-resource-kind-reference\
  \ for details supported values for kind.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: Site
---
