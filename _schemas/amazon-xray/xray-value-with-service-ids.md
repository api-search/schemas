---
description: Information about a segment annotation.
layout: schema
name: ValueWithServiceIds
properties_list:
- description: ''
  name: AnnotationValue
  type: object
- description: ''
  name: ServiceIds
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-value-with-service-ids-schema.json
slug: xray-value-with-service-ids
source_filename: xray-value-with-service-ids-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnnotationValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnnotationValue\"\n        },\n        {\n          \"description\": \"Values of the annotation.\"\n        }\n      ]\n    },\n    \"ServiceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceIds\"\n        },\n        {\n          \"description\": \"Services to which the annotation applies.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about a segment annotation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValueWithServiceIds\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-value-with-service-ids-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-value-with-service-ids-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ValueWithServiceIds
---
