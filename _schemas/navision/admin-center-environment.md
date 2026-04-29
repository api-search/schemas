---
description: ''
layout: schema
name: Environment
properties_list:
- description: Display name of the environment
  name: friendlyName
  type: string
- description: Environment type
  name: type
  type: string
- description: Environment name, unique within an application family
  name: name
  type: string
- description: Country/region code where the environment is deployed
  name: countryCode
  type: string
- description: Family of the environment application
  name: applicationFamily
  type: string
- description: Microsoft Entra tenant ID that owns the environment
  name: aadTenantId
  type: string
- description: Current status of the environment
  name: status
  type: string
- description: URL to log into the environment
  name: webClientLoginUrl
  type: string
- description: URL to access the environment service API
  name: webServiceUrl
  type: string
- description: Azure region where the database is stored
  name: locationName
  type: string
- description: Azure geo where the database is stored
  name: geoName
  type: string
- description: Logical ring group name (e.g., Prod, Preview)
  name: ringName
  type: string
- description: Application Insights instrumentation key
  name: appInsightsKey
  type: string
- description: When the environment was soft deleted
  name: softDeletedOn
  type: string
- description: When the environment will be permanently deleted
  name: hardDeletePendingOn
  type: string
- description: Reason the environment was deleted
  name: deleteReason
  type: string
- description: Update cadence for installed AppSource apps
  name: appSourceAppsUpdateCadence
  type: string
- description: ''
  name: versionDetails
  type: object
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-environment-schema.json
slug: admin-center-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Environment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"friendlyName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the environment\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Environment type\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Environment name, unique within an application family\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country/region code where the environment is deployed\"\n    },\n    \"applicationFamily\": {\n      \"type\": \"string\",\n      \"description\": \"Family of the environment application\"\n    },\n    \"aadTenantId\": {\n      \"type\": \"string\",\n      \"description\": \"Microsoft Entra tenant ID that owns the environment\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Current status of the environment\"\n    },\n    \"webClientLoginUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to log into the environment\"\n    },\n    \"webServiceUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to access the environment service API\"\n    },\n    \"locationName\": {\n      \"type\": \"string\",\n      \"description\": \"Azure region where the database is stored\"\n    },\n    \"geoName\": {\n      \"type\": \"string\",\n      \"description\": \"Azure geo where the database is stored\"\n    },\n    \"ringName\": {\n      \"type\": \"string\",\n      \"description\": \"Logical ring group name (e.g., Prod, Preview)\"\n    },\n    \"appInsightsKey\": {\n      \"type\": \"string\",\n      \"description\": \"Application Insights instrumentation key\"\n    },\n    \"softDeletedOn\": {\n      \"type\": \"string\",\n      \"description\": \"When the environment was soft deleted\"\n    },\n    \"hardDeletePendingOn\": {\n      \"\
  type\": \"string\",\n      \"description\": \"When the environment will be permanently deleted\"\n    },\n    \"deleteReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason the environment was deleted\"\n    },\n    \"appSourceAppsUpdateCadence\": {\n      \"type\": \"string\",\n      \"description\": \"Update cadence for installed AppSource apps\"\n    },\n    \"versionDetails\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-environment-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Environment
---
