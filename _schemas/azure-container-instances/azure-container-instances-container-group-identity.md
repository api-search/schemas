---
description: Identity for the container group.
layout: schema
name: ContainerGroupIdentity
properties_list:
- description: The principal id of the container group identity. This property will only be provided for a system assigned identity.
  name: principalId
  type: string
- description: The tenant id associated with the container group. This property will only be provided for a system assigned identity.
  name: tenantId
  type: string
- description: The type of identity used for the container group. The type 'SystemAssigned, UserAssigned' includes both an implicitly created identity and a set of user assigned identities. The type 'None' will remo
  name: type
  type: string
- description: 'The list of user identities associated with the container group. The user identity dictionary key references will be ARM resource ids in the form: ''/subscriptions/{subscriptionId}/resourceGroups/{reso'
  name: userAssignedIdentities
  type: object
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-group-identity-schema.json
slug: azure-container-instances-container-group-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-group-identity-schema.json\",\n  \"title\": \"ContainerGroupIdentity\",\n  \"description\": \"Identity for the container group.\",\n  \"properties\": {\n    \"principalId\": {\n      \"description\": \"The principal id of the container group identity. This property will only be provided for a system assigned identity.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"tenantId\": {\n      \"description\": \"The tenant id associated with the container group. This property will only be provided for a system assigned identity.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of identity used for the container group. The type 'SystemAssigned, UserAssigned' includes both an\
  \ implicitly created identity and a set of user assigned identities. The type 'None' will remove any identities from the container group.\",\n      \"enum\": [\n        \"SystemAssigned\",\n        \"UserAssigned\",\n        \"SystemAssigned, UserAssigned\",\n        \"None\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"ResourceIdentityType\"\n      }\n    },\n    \"userAssignedIdentities\": {\n      \"additionalProperties\": {\n        \"properties\": {\n          \"clientId\": {\n            \"description\": \"The client id of user assigned identity.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n          },\n          \"principalId\": {\n            \"description\": \"The principal id of user assigned identity.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"description\": \"The list of user\
  \ identities associated with the container group. The user identity dictionary key references will be ARM resource ids in the form: '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.\",\n      \"type\": \"object\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-group-identity-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerGroupIdentity
---
