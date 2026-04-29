---
description: GenerateConnectionRequest schema from Ampersand API
layout: schema
name: GenerateConnectionRequest
properties_list: []
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-generate-connection-request-schema.json
slug: ampersand-api-generate-connection-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-generate-connection-request-schema.json\",\n  \"title\": \"GenerateConnectionRequest\",\n  \"description\": \"GenerateConnectionRequest schema from Ampersand API\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/ConnectionRequest\"\n    },\n    {\n      \"type\": \"object\",\n      \"required\": [\n        \"groupRef\",\n        \"consumerRef\",\n        \"provider\"\n      ]\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-generate-connection-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: GenerateConnectionRequest
---
