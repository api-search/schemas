---
description: The result of a remote request signing operation.
layout: schema
name: RemoteSignResult
properties_list:
- description: ''
  name: uri
  type: string
- description: ''
  name: headers
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-remote-sign-result-schema.json
slug: rest-catalog-open-api-remote-sign-result
source_filename: rest-catalog-open-api-remote-sign-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remote-sign-result-schema.json\",\n  \"title\": \"RemoteSignResult\",\n  \"description\": \"The result of a remote request signing operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\"\n    },\n    \"headers\": {\n      \"$ref\": \"#/components/schemas/MultiValuedMap\"\n    }\n  },\n  \"required\": [\n    \"uri\",\n    \"headers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remote-sign-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RemoteSignResult
---
