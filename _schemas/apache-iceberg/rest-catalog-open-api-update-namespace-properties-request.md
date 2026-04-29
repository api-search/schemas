---
description: UpdateNamespacePropertiesRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: UpdateNamespacePropertiesRequest
properties_list:
- description: ''
  name: removals
  type: array
- description: ''
  name: updates
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-update-namespace-properties-request-schema.json
slug: rest-catalog-open-api-update-namespace-properties-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-update-namespace-properties-request-schema.json\",\n  \"title\": \"UpdateNamespacePropertiesRequest\",\n  \"description\": \"UpdateNamespacePropertiesRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"removals\": {\n      \"type\": \"array\",\n      \"uniqueItems\": true,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"department\",\n        \"access_group\"\n      ]\n    },\n    \"updates\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"owner\": \"Hank Bendickson\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-update-namespace-properties-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: UpdateNamespacePropertiesRequest
---
