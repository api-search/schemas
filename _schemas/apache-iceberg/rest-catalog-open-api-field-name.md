---
description: A full field name (including parent field names), such as those passed in APIs like Java `Schema#findField(String name)`. The nested field name follows these rules - Nested struct fields are named by concatenating field names at each struct level using dot (`.`) delimiter, e.g. employer.contact_info.address.zip_code - Nested fields in a map key are named using the keyword `key`, e.g. employee_address_map.key.first_name - Nested fields in a map value are named using the keyword `value`, e.g. employee_address_map.value.zip_code - Nested fields in a list are named using the keyword `element`, e.g. employees.element.first_name
layout: schema
name: FieldName
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-field-name-schema.json
slug: rest-catalog-open-api-field-name
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: FieldName
---
