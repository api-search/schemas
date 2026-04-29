---
description: JwksResponse schema from Backstage auth API
layout: schema
name: JwksResponse
properties_list:
- description: ''
  name: keys
  type: array
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/auth-jwks-response-schema.json
slug: auth-jwks-response
source_filename: auth-jwks-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/auth-jwks-response-schema.json\",\n  \"title\": \"JwksResponse\",\n  \"description\": \"JwksResponse schema from Backstage auth API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"kty\": {\n            \"type\": \"string\"\n          },\n          \"kid\": {\n            \"type\": \"string\"\n          },\n          \"alg\": {\n            \"type\": \"string\"\n          },\n          \"use\": {\n            \"type\": \"string\"\n          },\n          \"n\": {\n            \"type\": \"string\"\n          },\n          \"e\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/auth-jwks-response-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: JwksResponse
---
