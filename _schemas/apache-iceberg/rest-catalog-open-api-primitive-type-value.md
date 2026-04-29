---
description: PrimitiveTypeValue schema from Apache Iceberg REST Catalog API
layout: schema
name: PrimitiveTypeValue
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-primitive-type-value-schema.json
slug: rest-catalog-open-api-primitive-type-value
source_filename: rest-catalog-open-api-primitive-type-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-primitive-type-value-schema.json\",\n  \"title\": \"PrimitiveTypeValue\",\n  \"description\": \"PrimitiveTypeValue schema from Apache Iceberg REST Catalog API\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BooleanTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/IntegerTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/LongTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/FloatTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/DoubleTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/DecimalTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/StringTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/UUIDTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/DateTypeValue\"\
  \n    },\n    {\n      \"$ref\": \"#/components/schemas/TimeTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/TimestampTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/TimestampTzTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/TimestampNanoTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/TimestampTzNanoTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/FixedTypeValue\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/BinaryTypeValue\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-primitive-type-value-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PrimitiveTypeValue
---
