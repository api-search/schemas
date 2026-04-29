---
description: DeleteFile schema from Apache Iceberg REST Catalog API
layout: schema
name: DeleteFile
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-delete-file-schema.json
slug: rest-catalog-open-api-delete-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-delete-file-schema.json\",\n  \"title\": \"DeleteFile\",\n  \"description\": \"DeleteFile schema from Apache Iceberg REST Catalog API\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/PositionDeleteFile\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/EqualityDeleteFile\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-delete-file-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: DeleteFile
---
