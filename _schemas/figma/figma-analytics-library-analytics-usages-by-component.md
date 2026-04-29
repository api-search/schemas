---
description: Library analytics usage data broken down by component.
layout: schema
name: LibraryAnalyticsUsagesByComponent
properties_list:
- description: Unique, stable id of the component.
  name: componentKey
  type: string
- description: Name of the component.
  name: componentName
  type: string
- description: Unique, stable id of the component set that this component belongs to.
  name: componentSetKey
  type: string
- description: Name of the component set that this component belongs to.
  name: componentSetName
  type: string
- description: The number of instances of the component within the organization.
  name: numInstances
  type: number
- description: The number of teams using the component within the organization.
  name: numTeamsUsing
  type: number
- description: The number of files using the component within the organization.
  name: numFilesUsing
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-analytics-library-analytics-usages-by-component-schema.json
slug: figma-analytics-library-analytics-usages-by-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryAnalyticsUsagesByComponent\",\n  \"type\": \"object\",\n  \"description\": \"Library analytics usage data broken down by component.\",\n  \"properties\": {\n    \"componentKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique, stable id of the component.\"\n    },\n    \"componentName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the component.\"\n    },\n    \"componentSetKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique, stable id of the component set that this component belongs to.\"\n    },\n    \"componentSetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the component set that this component belongs to.\"\n    },\n    \"numInstances\": {\n      \"type\": \"number\",\n      \"description\": \"The number of instances of the component within the organization.\"\n    },\n    \"numTeamsUsing\": {\n \
  \     \"type\": \"number\",\n      \"description\": \"The number of teams using the component within the organization.\"\n    },\n    \"numFilesUsing\": {\n      \"type\": \"number\",\n      \"description\": \"The number of files using the component within the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-analytics-library-analytics-usages-by-component-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: LibraryAnalyticsUsagesByComponent
---
