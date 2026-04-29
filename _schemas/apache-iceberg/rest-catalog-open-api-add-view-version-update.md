---
description: AddViewVersionUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: AddViewVersionUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: view-version
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-add-view-version-update-schema.json
slug: rest-catalog-open-api-add-view-version-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-view-version-update-schema.json\",\n  \"title\": \"AddViewVersionUpdate\",\n  \"description\": \"AddViewVersionUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"add-view-version\"\n    },\n    \"view-version\": {\n      \"$ref\": \"#/components/schemas/ViewVersion\"\n    }\n  },\n  \"required\": [\n    \"view-version\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-view-version-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AddViewVersionUpdate
---
