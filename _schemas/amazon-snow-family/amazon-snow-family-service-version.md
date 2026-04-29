---
description: The version of the requested service.
layout: schema
name: ServiceVersion
properties_list:
- description: ''
  name: Version
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-service-version-schema.json
slug: amazon-snow-family-service-version
source_filename: amazon-snow-family-service-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-service-version-schema.json\",\n  \"title\": \"ServiceVersion\",\n  \"description\": \"The version of the requested service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The version number of the requested service.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-service-version-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ServiceVersion
---
