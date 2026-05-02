---
description: Represents an Azure Resource Manager resource group, which is a container that holds related resources for an Azure solution. The resource group includes resources that you want to manage as a group.
layout: schema
name: Azure Resource Group
properties_list:
- description: The fully qualified resource ID for the resource group
  name: id
  type: string
- description: The name of the resource group
  name: name
  type: string
- description: The type of the resource (Microsoft.Resources/resourceGroups)
  name: type
  type: string
- description: The location of the resource group. It cannot be changed after creation.
  name: location
  type: string
- description: The ID of the resource that manages this resource group
  name: managedBy
  type:
  - string
  - 'null'
- description: The tags attached to the resource group
  name: tags
  type:
  - object
  - 'null'
- description: The resource group properties
  name: properties
  type: object
provider_name: Microsoft
provider_slug: microsoft
schema_file: json-schema/microsoft-azure-resource-group-schema.json
slug: microsoft-azure-resource-group
source_filename: microsoft-azure-resource-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/rest/api/schemas/microsoft/azure-resource-group.json\",\n  \"title\": \"Azure Resource Group\",\n  \"description\": \"Represents an Azure Resource Manager resource group, which is a container that holds related resources for an Azure solution. The resource group includes resources that you want to manage as a group.\",\n  \"type\": \"object\",\n  \"required\": [\"location\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified resource ID for the resource group\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource group\",\n      \"readOnly\": true,\n      \"pattern\": \"^[-\\\\w._()]+$\",\n      \"maxLength\": 90\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource (Microsoft.Resources/resourceGroups)\"\
  ,\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the resource group. It cannot be changed after creation.\"\n    },\n    \"managedBy\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the resource that manages this resource group\"\n    },\n    \"tags\": {\n      \"type\": [\"object\", \"null\"],\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The tags attached to the resource group\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The resource group properties\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"The provisioning state of the resource group\",\n          \"readOnly\": true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/json-schema/microsoft-azure-resource-group-schema.json
tags: []
title: Azure Resource Group
---
