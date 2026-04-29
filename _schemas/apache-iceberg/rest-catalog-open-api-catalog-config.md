---
description: Server-provided configuration for the catalog.
layout: schema
name: CatalogConfig
properties_list:
- description: Properties that should be used to override client configuration; applied after defaults and client configuration.
  name: overrides
  type: object
- description: Properties that should be used as default configuration; applied before client configuration.
  name: defaults
  type: object
- description: A list of endpoints that the server supports. The format of each endpoint must be "<HTTP verb> <resource path from OpenAPI REST spec>". The HTTP verb and the resource path must be separated by a space
  name: endpoints
  type: array
- description: Client reuse window for an Idempotency-Key (ISO-8601 duration, e.g., PT30M, PT24H). Interpreted as the maximum time from the first submission using a key to the last retry during which a client may re
  name: idempotency-key-lifetime
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-catalog-config-schema.json
slug: rest-catalog-open-api-catalog-config
source_filename: rest-catalog-open-api-catalog-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-catalog-config-schema.json\",\n  \"title\": \"CatalogConfig\",\n  \"description\": \"Server-provided configuration for the catalog.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"overrides\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Properties that should be used to override client configuration; applied after defaults and client configuration.\"\n    },\n    \"defaults\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Properties that should be used as default configuration; applied before client configuration.\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"string\"\n      },\n      \"description\": \"A list of endpoints that the server supports. The format of each endpoint must be \\\"<HTTP verb> <resource path from OpenAPI REST spec>\\\". The HTTP verb and the resource path must be separated by a space character.\",\n      \"example\": [\n        \"GET /v1/{prefix}/namespaces/{namespace}\",\n        \"GET /v1/{prefix}/namespaces\",\n        \"POST /v1/{prefix}/namespaces\",\n        \"GET /v1/{prefix}/namespaces/{namespace}/tables/{table}\",\n        \"GET /v1/{prefix}/namespaces/{namespace}/views/{view}\"\n      ]\n    },\n    \"idempotency-key-lifetime\": {\n      \"type\": \"string\",\n      \"format\": \"duration\",\n      \"description\": \"Client reuse window for an Idempotency-Key (ISO-8601 duration, e.g., PT30M, PT24H). Interpreted as the maximum time from the first submission using a key to the last retry during which a client may reuse that key. Servers SHOULD accept retries for at least this duration and MAY include\
  \ a grace period to account for delays/clock skew. Clients SHOULD NOT reuse an Idempotency-Key after this window elapses; they SHOULD generate a new key for any subsequent attempt. Presence of this field indicates the server supports Idempotency-Key semantics for mutation endpoints. If absent, clients MUST assume idempotency is not supported.\",\n      \"example\": \"PT30M\"\n    }\n  },\n  \"required\": [\n    \"defaults\",\n    \"overrides\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-catalog-config-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CatalogConfig
---
