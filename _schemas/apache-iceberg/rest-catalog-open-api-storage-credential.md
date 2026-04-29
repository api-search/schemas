---
description: StorageCredential schema from Apache Iceberg REST Catalog API
layout: schema
name: StorageCredential
properties_list:
- description: Indicates a storage location prefix where the credential is relevant. Clients should choose the most specific prefix (by selecting the longest prefix) if several credentials of the same type are avail
  name: prefix
  type: string
- description: ''
  name: config
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-storage-credential-schema.json
slug: rest-catalog-open-api-storage-credential
source_filename: rest-catalog-open-api-storage-credential-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-storage-credential-schema.json\",\n  \"title\": \"StorageCredential\",\n  \"description\": \"StorageCredential schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates a storage location prefix where the credential is relevant. Clients should choose the most specific prefix (by selecting the longest prefix) if several credentials of the same type are available.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"prefix\",\n    \"config\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-storage-credential-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: StorageCredential
---
