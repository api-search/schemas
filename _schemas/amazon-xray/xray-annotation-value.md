---
description: 'Value of a segment annotation. Has one of three value types: Number, Boolean, or String.'
layout: schema
name: AnnotationValue
properties_list:
- description: ''
  name: NumberValue
  type: object
- description: ''
  name: BooleanValue
  type: object
- description: ''
  name: StringValue
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-annotation-value-schema.json
slug: xray-annotation-value
source_filename: xray-annotation-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"NumberValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"Value for a Number annotation.\"\n        }\n      ]\n    },\n    \"BooleanValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Value for a Boolean annotation.\"\n        }\n      ]\n    },\n    \"StringValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Value for a String annotation.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Value of a segment annotation. Has one of three value types: Number, Boolean, or String.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnnotationValue\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-annotation-value-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-annotation-value-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: AnnotationValue
---
