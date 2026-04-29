---
description: Decimal type values are serialized as strings. Decimals with a positive scale serialize as numeric plain text, while decimals with a negative scale use scientific notation and the exponent will be equal to the negated scale. For instance, a decimal with a positive scale is '123.4500', with zero scale is '2', and with a negative scale is '2E+20'
layout: schema
name: DecimalTypeValue
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-decimal-type-value-schema.json
slug: rest-catalog-open-api-decimal-type-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-decimal-type-value-schema.json\",\n  \"title\": \"DecimalTypeValue\",\n  \"description\": \"Decimal type values are serialized as strings. Decimals with a positive scale serialize as numeric plain text, while decimals with a negative scale use scientific notation and the exponent will be equal to the negated scale. For instance, a decimal with a positive scale is '123.4500', with zero scale is '2', and with a negative scale is '2E+20'\",\n  \"type\": \"string\",\n  \"example\": \"123.4500\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-decimal-type-value-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: DecimalTypeValue
---
