---
description: Library analytics usage data broken down by file.
layout: schema
name: LibraryAnalyticsUsagesByFile
properties_list:
- description: The name of the file using the library.
  name: fileName
  type: string
- description: The name of the team the file belongs to.
  name: teamName
  type: string
- description: The name of the workspace that the file belongs to.
  name: workspaceName
  type: string
- description: The number of component instances from the library used within the file.
  name: numInstances
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-analytics-library-analytics-usages-by-file-schema.json
slug: figma-analytics-library-analytics-usages-by-file
source_filename: figma-analytics-library-analytics-usages-by-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryAnalyticsUsagesByFile\",\n  \"type\": \"object\",\n  \"description\": \"Library analytics usage data broken down by file.\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file using the library.\"\n    },\n    \"teamName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the team the file belongs to.\"\n    },\n    \"workspaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workspace that the file belongs to.\"\n    },\n    \"numInstances\": {\n      \"type\": \"number\",\n      \"description\": \"The number of component instances from the library used within the file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-analytics-library-analytics-usages-by-file-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: LibraryAnalyticsUsagesByFile
---
