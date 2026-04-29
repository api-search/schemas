---
description: A resource group is a container that holds related resources for an Azure solution. The resource group can include all the resources for the solution, or only those resources that you want to manage as a group. Resource groups are used to organize resources by lifecycle and security boundary.
layout: schema
name: Azure Resource Group
properties_list:
- description: 'The ID of the resource group. Format: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}.'
  name: id
  type: string
- description: The name of the resource group.
  name: name
  type: string
- description: The type of the resource group.
  name: type
  type: string
- description: The location of the resource group. It cannot be changed after the resource group has been created. It must be one of the supported Azure locations.
  name: location
  type: string
- description: The ID of the resource that manages this resource group.
  name: managedBy
  type: string
- description: The tags attached to the resource group.
  name: tags
  type: object
- description: The resource group properties.
  name: properties
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/microsoft-azure-resource-group-schema.json
slug: microsoft-azure-resource-group
source_filename: microsoft-azure-resource-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-azure/resource-group\",\n  \"title\": \"Azure Resource Group\",\n  \"description\": \"A resource group is a container that holds related resources for an Azure solution. The resource group can include all the resources for the solution, or only those resources that you want to manage as a group. Resource groups are used to organize resources by lifecycle and security boundary.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the resource group. Format: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/myResourceGroup\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource group.\"\
  ,\n      \"readOnly\": true,\n      \"minLength\": 1,\n      \"maxLength\": 90,\n      \"examples\": [\n        \"myResourceGroup\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource group.\",\n      \"readOnly\": true,\n      \"const\": \"Microsoft.Resources/resourceGroups\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the resource group. It cannot be changed after the resource group has been created. It must be one of the supported Azure locations.\",\n      \"examples\": [\n        \"eastus\",\n        \"westus2\",\n        \"westeurope\"\n      ]\n    },\n    \"managedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the resource that manages this resource group.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags attached to the resource group.\",\n      \"additionalProperties\": {\n        \"type\": \"\
  string\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The resource group properties.\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"The provisioning state of the resource group.\",\n          \"readOnly\": true,\n          \"examples\": [\n            \"Succeeded\",\n            \"Deleting\",\n            \"Failed\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"location\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/microsoft-azure-resource-group-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Azure Resource Group
---
