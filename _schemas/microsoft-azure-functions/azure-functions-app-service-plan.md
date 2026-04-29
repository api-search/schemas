---
description: App Service plan.
layout: schema
name: AppServicePlan
properties_list:
- description: AppServicePlan resource specific properties
  name: properties
  type: object
- description: Description of a SKU for a scalable resource.
  name: sku
  type: object
- description: Extended Location.
  name: extendedLocation
  type: object
- description: Kind of resource. If the resource is an app, you can refer to https://github.com/Azure/app-service-linux-docs/blob/master/Things_You_Should_Know/kind_property.md#app-service-resource-kind-reference fo
  name: kind
  type: string
- description: Managed service identity.
  name: identity
  type: object
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-app-service-plan-schema.json
slug: azure-functions-app-service-plan
source_filename: azure-functions-app-service-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-app-service-plan-schema.json\",\n  \"title\": \"AppServicePlan\",\n  \"description\": \"App Service plan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/AppServicePlanProperties\",\n      \"description\": \"AppServicePlan resource specific properties\",\n      \"x-ms-client-flatten\": true\n    },\n    \"sku\": {\n      \"$ref\": \"#/definitions/SkuDescription\",\n      \"description\": \"Description of a SKU for a scalable resource.\"\n    },\n    \"extendedLocation\": {\n      \"$ref\": \"#/definitions/ExtendedLocation\",\n      \"description\": \"Extended Location.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of resource. If the resource is an app, you can refer to https://github.com/Azure/app-service-linux-docs/blob/master/Things_You_Should_Know/kind_property.md#app-service-resource-kind-reference\
  \ for details supported values for kind.\"\n    },\n    \"identity\": {\n      \"$ref\": \"#/definitions/ManagedServiceIdentity\",\n      \"description\": \"Managed service identity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-app-service-plan-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: AppServicePlan
---
