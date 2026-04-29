---
description: ViewUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: ViewUpdate
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-view-update-schema.json
slug: rest-catalog-open-api-view-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-update-schema.json\",\n  \"title\": \"ViewUpdate\",\n  \"description\": \"ViewUpdate schema from Apache Iceberg REST Catalog API\",\n  \"anyOf\": [\n    {\n      \"$ref\": \"#/components/schemas/AssignUUIDUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/UpgradeFormatVersionUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/AddSchemaUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetLocationUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetPropertiesUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemovePropertiesUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/AddViewVersionUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetCurrentViewVersionUpdate\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ViewUpdate
---
