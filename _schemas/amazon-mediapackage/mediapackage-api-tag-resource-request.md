---
description: TagResourceRequest schema from Amazon MediaPackage API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-tag-resource-request-schema.json
slug: mediapackage-api-tag-resource-request
source_filename: mediapackage-api-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon MediaPackage API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-tag-resource-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: TagResourceRequest
---
