---
description: SignedUrl schema from Ampersand API
layout: schema
name: SignedUrl
properties_list:
- description: The signed URL to upload the zip file to.
  name: url
  type: string
- description: The bucket (will match the bucket part of the url).
  name: bucket
  type: string
- description: The path (will match the path part of the url).
  name: path
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-signed-url-schema.json
slug: ampersand-api-signed-url
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-signed-url-schema.json\",\n  \"title\": \"SignedUrl\",\n  \"description\": \"SignedUrl schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The signed URL to upload the zip file to.\"\n    },\n    \"bucket\": {\n      \"type\": \"string\",\n      \"description\": \"The bucket (will match the bucket part of the url).\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path (will match the path part of the url).\"\n    }\n  },\n  \"required\": [\n    \"url\",\n    \"bucket\",\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-signed-url-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: SignedUrl
---
