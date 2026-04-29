---
description: A tag is a label consisting of a user-defined key and value. The form for tags is {"Key", "Value"}
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-tag-schema.json
slug: healthlake-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ],\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \" The key portion of a tag. Tag keys are case sensitive. \"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \" The value portion of a tag. Tag values are case sensitive. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" A tag is a label consisting of a user-defined key and value. The form for tags is {\\\"Key\\\", \\\"Value\\\"} \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-tag-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: Tag
---
