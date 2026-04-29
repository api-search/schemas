---
description: POST body for creating/updating organization level OAuth credentials
layout: schema
name: OrganizationOAuthCredentialsRequest
properties_list:
- description: ''
  name: actorType
  type: object
- description: The name of the source i.e. google-ads
  name: name
  type: string
- description: ''
  name: configuration
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-organization-o-auth-credentials-request-schema.json
slug: airbyte-organization-o-auth-credentials-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-organization-o-auth-credentials-request-schema.json\",\n  \"title\": \"OrganizationOAuthCredentialsRequest\",\n  \"description\": \"POST body for creating/updating organization level OAuth credentials\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actorType\": {\n      \"$ref\": \"#/components/schemas/ActorTypeEnum\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the source i.e. google-ads\"\n    },\n    \"configuration\": {\n      \"$ref\": \"#/components/schemas/OAuthCredentialsConfiguration\"\n    }\n  },\n  \"required\": [\n    \"actorType\",\n    \"name\",\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-organization-o-auth-credentials-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: OrganizationOAuthCredentialsRequest
---
