---
description: SetCurrentViewVersionUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetCurrentViewVersionUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: The view version id to set as current, or -1 to set last added view version id
  name: view-version-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-current-view-version-update-schema.json
slug: rest-catalog-open-api-set-current-view-version-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-current-view-version-update-schema.json\",\n  \"title\": \"SetCurrentViewVersionUpdate\",\n  \"description\": \"SetCurrentViewVersionUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"set-current-view-version\"\n    },\n    \"view-version-id\": {\n      \"type\": \"integer\",\n      \"description\": \"The view version id to set as current, or -1 to set last added view version id\"\n    }\n  },\n  \"required\": [\n    \"view-version-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-current-view-version-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetCurrentViewVersionUpdate
---
