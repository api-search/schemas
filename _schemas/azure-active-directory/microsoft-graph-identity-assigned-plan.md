---
description: Represents a plan assigned to a user.
layout: schema
name: AssignedPlan
properties_list:
- description: ''
  name: assignedDateTime
  type: string
- description: ''
  name: capabilityStatus
  type: string
- description: ''
  name: service
  type: string
- description: ''
  name: servicePlanId
  type: string
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-assigned-plan-schema.json
slug: microsoft-graph-identity-assigned-plan
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssignedPlan\",\n  \"type\": \"object\",\n  \"description\": \"Represents a plan assigned to a user.\",\n  \"properties\": {\n    \"assignedDateTime\": {\n      \"type\": \"string\"\n    },\n    \"capabilityStatus\": {\n      \"type\": \"string\"\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"servicePlanId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-assigned-plan-schema.json
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
title: AssignedPlan
---
