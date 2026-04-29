---
description: CreateNamespaceResponse schema from Apache Iceberg REST Catalog API
layout: schema
name: CreateNamespaceResponse
properties_list:
- description: ''
  name: namespace
  type: object
- description: Properties stored on the namespace, if supported by the server.
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-create-namespace-response-schema.json
slug: rest-catalog-open-api-create-namespace-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-namespace-response-schema.json\",\n  \"title\": \"CreateNamespaceResponse\",\n  \"description\": \"CreateNamespaceResponse schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"$ref\": \"#/components/schemas/Namespace\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Properties stored on the namespace, if supported by the server.\",\n      \"example\": {\n        \"owner\": \"Ralph\",\n        \"created_at\": \"1452120468\"\n      },\n      \"default\": {}\n    }\n  },\n  \"required\": [\n    \"namespace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-namespace-response-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CreateNamespaceResponse
---
