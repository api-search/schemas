---
description: LoadCredentialsResponse schema from Apache Iceberg REST Catalog API
layout: schema
name: LoadCredentialsResponse
properties_list:
- description: ''
  name: storage-credentials
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-load-credentials-response-schema.json
slug: rest-catalog-open-api-load-credentials-response
source_filename: rest-catalog-open-api-load-credentials-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-load-credentials-response-schema.json\",\n  \"title\": \"LoadCredentialsResponse\",\n  \"description\": \"LoadCredentialsResponse schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storage-credentials\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageCredential\"\n      }\n    }\n  },\n  \"required\": [\n    \"storage-credentials\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-load-credentials-response-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: LoadCredentialsResponse
---
