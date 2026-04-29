---
description: UUID type values are serialized as a 36-character lowercase string in standard UUID format as specified by RFC-4122
layout: schema
name: UUIDTypeValue
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-uuid-type-value-schema.json
slug: rest-catalog-open-api-uuid-type-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-uuid-type-value-schema.json\",\n  \"title\": \"UUIDTypeValue\",\n  \"description\": \"UUID type values are serialized as a 36-character lowercase string in standard UUID format as specified by RFC-4122\",\n  \"type\": \"string\",\n  \"format\": \"uuid\",\n  \"pattern\": \"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$\",\n  \"minLength\": 36,\n  \"maxLength\": 36,\n  \"example\": \"eb26bdb1-a1d8-4aa6-990e-da940875492c\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-uuid-type-value-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: UUIDTypeValue
---
