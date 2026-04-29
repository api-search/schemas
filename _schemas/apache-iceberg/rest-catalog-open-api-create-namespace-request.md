---
description: CreateNamespaceRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: CreateNamespaceRequest
properties_list:
- description: ''
  name: namespace
  type: object
- description: Configured string to string map of properties for the namespace
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-create-namespace-request-schema.json
slug: rest-catalog-open-api-create-namespace-request
source_filename: rest-catalog-open-api-create-namespace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-namespace-request-schema.json\",\n  \"title\": \"CreateNamespaceRequest\",\n  \"description\": \"CreateNamespaceRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"$ref\": \"#/components/schemas/Namespace\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Configured string to string map of properties for the namespace\",\n      \"example\": {\n        \"owner\": \"Hank Bendickson\"\n      },\n      \"default\": {},\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"namespace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-namespace-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CreateNamespaceRequest
---
