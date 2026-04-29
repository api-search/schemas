---
description: Managed identity for the resource.
layout: schema
name: IdentityProperties
properties_list:
- description: The principal ID of resource identity.
  name: principalId
  type: string
- description: The tenant ID of resource.
  name: tenantId
  type: string
- description: The identity type.
  name: type
  type: string
- description: 'The list of user identities associated with the resource. The user identity dictionary key references will be ARM resource ids in the form: ''/subscriptions/{subscriptionId}/resourceGroups/{resourceGro'
  name: userAssignedIdentities
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-identity-properties-schema.json
slug: azure-container-registry-identity-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-identity-properties-schema.json\",\n  \"title\": \"IdentityProperties\",\n  \"description\": \"Managed identity for the resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"principalId\": {\n      \"description\": \"The principal ID of resource identity.\",\n      \"type\": \"string\"\n    },\n    \"tenantId\": {\n      \"description\": \"The tenant ID of resource.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The identity type.\",\n      \"enum\": [\n        \"SystemAssigned\",\n        \"UserAssigned\",\n        \"SystemAssigned, UserAssigned\",\n        \"None\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"ResourceIdentityType\"\n      }\n    },\n\
  \    \"userAssignedIdentities\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/UserIdentityProperties\"\n      },\n      \"description\": \"The list of user identities associated with the resource. The user identity \\r\\ndictionary key references will be ARM resource ids in the form: \\r\\n'/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/\\r\\n    providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.\",\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-identity-properties-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: IdentityProperties
---
