---
description: UpdateNamespacePropertiesResponse schema from Apache Iceberg REST Catalog API
layout: schema
name: UpdateNamespacePropertiesResponse
properties_list:
- description: List of property keys that were added or updated
  name: updated
  type: array
- description: List of properties that were removed
  name: removed
  type: array
- description: List of properties requested for removal that were not found in the namespace's properties. Represents a partial success response. Server's do not need to implement this.
  name: missing
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-update-namespace-properties-response-schema.json
slug: rest-catalog-open-api-update-namespace-properties-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-update-namespace-properties-response-schema.json\",\n  \"title\": \"UpdateNamespacePropertiesResponse\",\n  \"description\": \"UpdateNamespacePropertiesResponse schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updated\": {\n      \"description\": \"List of property keys that were added or updated\",\n      \"type\": \"array\",\n      \"uniqueItems\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"removed\": {\n      \"description\": \"List of properties that were removed\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"missing\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"\
  List of properties requested for removal that were not found in the namespace's properties. Represents a partial success response. Server's do not need to implement this.\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"updated\",\n    \"removed\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-update-namespace-properties-response-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: UpdateNamespacePropertiesResponse
---
