---
description: An application package available for installation in a Power Platform environment.
layout: schema
name: ApplicationPackage
properties_list:
- description: The unique identifier of the application package.
  name: id
  type: string
- description: The unique name of the application package.
  name: uniqueName
  type: string
- description: The version of the application package.
  name: version
  type: string
- description: A localized description of the application package.
  name: localizedDescription
  type: '[''string'', ''null'']'
- description: The localized display name of the application package.
  name: localizedName
  type: '[''string'', ''null'']'
- description: The visibility of the application.
  name: applicationVisibility
  type: string
- description: The current installation state of the package.
  name: state
  type: string
- description: Details about the last error if installation failed.
  name: lastError
  type: '[''object'', ''null'']'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-application-package-schema.json
slug: power-platform-application-package
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationPackage\",\n  \"type\": \"object\",\n  \"description\": \"An application package available for installation in a Power Platform environment.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application package.\"\n    },\n    \"uniqueName\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the application package.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the application package.\"\n    },\n    \"localizedDescription\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"A localized description of the application package.\"\n    },\n    \"localizedName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The localized display name of the application package.\"\n    },\n    \"applicationVisibility\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The visibility of the application.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current installation state of the package.\"\n    },\n    \"lastError\": {\n      \"type\": \"['object', 'null']\",\n      \"description\": \"Details about the last error if installation failed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-application-package-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: ApplicationPackage
---
