---
description: Assigning a UUID to a table/view should only be done when creating the table/view. It is not safe to re-assign the UUID if a table/view already has a UUID assigned
layout: schema
name: AssignUUIDUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: uuid
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assign-uuid-update-schema.json
slug: rest-catalog-open-api-assign-uuid-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assign-uuid-update-schema.json\",\n  \"title\": \"AssignUUIDUpdate\",\n  \"description\": \"Assigning a UUID to a table/view should only be done when creating the table/view. It is not safe to re-assign the UUID if a table/view already has a UUID assigned\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"assign-uuid\"\n    },\n    \"uuid\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"uuid\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-assign-uuid-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssignUUIDUpdate
---
