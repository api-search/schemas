---
description: ''
layout: schema
name: OAuth
properties_list:
- description: The client ID of the OAuth2 credential associated with the Polaris service connection.
  name: oauth_client_id
  type: string
- description: The secret for the OAuth2 credential associated with the Polaris service connection.
  name: oauth_client_secret
  type: string
- description: The scope of the OAuth token. Only one scope is included in the Iceberg REST API specification, but catalogs can support more than one scope in their implementation.
  name: oauth_allowed_scopes
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/catalog-integration-o-auth-schema.json
slug: catalog-integration-o-auth
source_filename: catalog-integration-o-auth-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OAuth\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"oauth_client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The client ID of the OAuth2 credential associated with the Polaris service connection.\"\n    },\n    \"oauth_client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"The secret for the OAuth2 credential associated with the Polaris service connection.\"\n    },\n    \"oauth_allowed_scopes\": {\n      \"type\": \"array\",\n      \"description\": \"The scope of the OAuth token. Only one scope is included in the Iceberg REST API specification, but catalogs can support more than one scope in their implementation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/catalog-integration-o-auth-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: OAuth
---
