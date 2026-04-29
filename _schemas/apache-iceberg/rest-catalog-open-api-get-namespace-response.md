---
description: GetNamespaceResponse schema from Apache Iceberg REST Catalog API
layout: schema
name: GetNamespaceResponse
properties_list:
- description: ''
  name: namespace
  type: object
- description: Properties stored on the namespace, if supported by the server. If the server does not support namespace properties, it should return null for this field. If namespace properties are supported, but no
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-get-namespace-response-schema.json
slug: rest-catalog-open-api-get-namespace-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-get-namespace-response-schema.json\",\n  \"title\": \"GetNamespaceResponse\",\n  \"description\": \"GetNamespaceResponse schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"$ref\": \"#/components/schemas/Namespace\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties stored on the namespace, if supported by the server. If the server does not support namespace properties, it should return null for this field. If namespace properties are supported, but none are set, it should return an empty object.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"owner\": \"Ralph\",\n        \"transient_lastDdlTime\": \"1452120468\"\
  \n      },\n      \"default\": {},\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"namespace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-get-namespace-response-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: GetNamespaceResponse
---
