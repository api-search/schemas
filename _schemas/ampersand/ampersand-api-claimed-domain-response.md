---
description: ClaimedDomainResponse schema from Ampersand API
layout: schema
name: ClaimedDomainResponse
properties_list:
- description: Unique identifier for the claimed domain
  name: id
  type: string
- description: Type of the parent entity that claimed the domain
  name: parentType
  type: string
- description: ID of the parent entity that claimed the domain
  name: parentId
  type: string
- description: The normalized domain name
  name: domain
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-claimed-domain-response-schema.json
slug: ampersand-api-claimed-domain-response
source_filename: ampersand-api-claimed-domain-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-claimed-domain-response-schema.json\",\n  \"title\": \"ClaimedDomainResponse\",\n  \"description\": \"ClaimedDomainResponse schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the claimed domain\",\n      \"example\": \"00000000-0000-0000-0000-000000000001\"\n    },\n    \"parentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the parent entity that claimed the domain\",\n      \"example\": \"org\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent entity that claimed the domain\",\n      \"example\": \"00000000-0000-0000-0000-000000000001\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The normalized domain name\",\n      \"example\": \"xyz.com\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"parentType\",\n    \"parentId\",\n    \"domain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-claimed-domain-response-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ClaimedDomainResponse
---
