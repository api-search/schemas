---
description: Token type identifier, from RFC 8693 Section 3 See https://datatracker.ietf.org/doc/html/rfc8693#section-3
layout: schema
name: TokenType
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-token-type-schema.json
slug: rest-catalog-open-api-token-type
source_filename: rest-catalog-open-api-token-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-token-type-schema.json\",\n  \"title\": \"TokenType\",\n  \"description\": \"Token type identifier, from RFC 8693 Section 3\\n\\nSee https://datatracker.ietf.org/doc/html/rfc8693#section-3\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"urn:ietf:params:oauth:token-type:access_token\",\n    \"urn:ietf:params:oauth:token-type:refresh_token\",\n    \"urn:ietf:params:oauth:token-type:id_token\",\n    \"urn:ietf:params:oauth:token-type:saml1\",\n    \"urn:ietf:params:oauth:token-type:saml2\",\n    \"urn:ietf:params:oauth:token-type:jwt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-token-type-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: TokenType
---
