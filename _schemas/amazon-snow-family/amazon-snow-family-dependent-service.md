---
description: The name and version of the service dependant on the requested service.
layout: schema
name: DependentService
properties_list:
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: ServiceVersion
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-dependent-service-schema.json
slug: amazon-snow-family-dependent-service
source_filename: amazon-snow-family-dependent-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-dependent-service-schema.json\",\n  \"title\": \"DependentService\",\n  \"description\": \"The name and version of the service dependant on the requested service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n          \"description\": \"The name of the dependent service.\"\n        }\n      ]\n    },\n    \"ServiceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceVersion\"\n        },\n        {\n          \"description\": \"The version of the dependent service.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-dependent-service-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DependentService
---
