---
description: CreateViewRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: CreateViewRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: schema
  type: object
- description: The view version to create, will replace the schema-id sent within the view-version with the id assigned to the provided schema
  name: view-version
  type: object
- description: ''
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-create-view-request-schema.json
slug: rest-catalog-open-api-create-view-request
source_filename: rest-catalog-open-api-create-view-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-view-request-schema.json\",\n  \"title\": \"CreateViewRequest\",\n  \"description\": \"CreateViewRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"schema\": {\n      \"$ref\": \"#/components/schemas/Schema\"\n    },\n    \"view-version\": {\n      \"$ref\": \"#/components/schemas/ViewVersion\",\n      \"description\": \"The view version to create, will replace the schema-id sent within the view-version with the id assigned to the provided schema\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n\
  \    \"name\",\n    \"schema\",\n    \"view-version\",\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-view-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CreateViewRequest
---
