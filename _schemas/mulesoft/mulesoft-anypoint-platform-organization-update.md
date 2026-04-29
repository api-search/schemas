---
description: Fields that can be updated on an organization
layout: schema
name: OrganizationUpdate
properties_list:
- description: Display name of the organization
  name: name
  type: string
- description: User ID of the new organization owner
  name: ownerId
  type: string
- description: Session timeout in minutes
  name: sessionTimeout
  type: integer
- description: Whether multi-factor authentication is required
  name: mfaRequired
  type: boolean
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-organization-update-schema.json
slug: mulesoft-anypoint-platform-organization-update
source_filename: mulesoft-anypoint-platform-organization-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrganizationUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Fields that can be updated on an organization\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the organization\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the new organization owner\"\n    },\n    \"sessionTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Session timeout in minutes\"\n    },\n    \"mfaRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether multi-factor authentication is required\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-organization-update-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: OrganizationUpdate
---
