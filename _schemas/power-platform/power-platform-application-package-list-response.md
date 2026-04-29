---
description: Response containing a list of application packages.
layout: schema
name: ApplicationPackageListResponse
properties_list:
- description: Array of application package resources.
  name: value
  type: array
- description: URL to retrieve the next page of results.
  name: '@odata.nextLink'
  type: '[''string'', ''null'']'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-application-package-list-response-schema.json
slug: power-platform-application-package-list-response
source_filename: power-platform-application-package-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationPackageListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response containing a list of application packages.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of application package resources.\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"URL to retrieve the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-application-package-list-response-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: ApplicationPackageListResponse
---
