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
