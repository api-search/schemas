---
description: Platform entitlements and resource limits for the organization
layout: schema
name: Entitlements
properties_list:
- description: Whether the organization can create new environments
  name: createEnvironments
  type: boolean
- description: Whether global deployment is enabled
  name: globalDeployment
  type: boolean
- description: Whether the organization can create sub-organizations
  name: createSubOrgs
  type: boolean
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-entitlements-schema.json
slug: mulesoft-anypoint-platform-entitlements
source_filename: mulesoft-anypoint-platform-entitlements-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Entitlements\",\n  \"type\": \"object\",\n  \"description\": \"Platform entitlements and resource limits for the organization\",\n  \"properties\": {\n    \"createEnvironments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization can create new environments\"\n    },\n    \"globalDeployment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether global deployment is enabled\"\n    },\n    \"createSubOrgs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization can create sub-organizations\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-entitlements-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: Entitlements
---
