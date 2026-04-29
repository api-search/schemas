---
description: TagList schema from AWS App Mesh
layout: schema
name: TagList
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-tag-list-schema.json
slug: app-mesh-tag-list
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagKey\"\n          },\n          {\n            \"description\": \"One part of a key-value pair that make up a tag. A <code>key</code> is a general label that acts like a category for more specific tag values.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          },\n          {\n            \"description\": \"The optional part of a key-value pair that make up a tag. A <code>value</code> acts as a descriptor within a tag category (key).\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"key\",\n      \"value\"\n    ],\n    \"description\": \"Optional metadata that you apply to a resource to assist with categorization and organization. Each tag consists of a key\
  \ and an optional value, both of which you define. Tag keys can have a maximum character length of 128 characters, and tag values can have a maximum length of 256 characters.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tag-list-schema.json\",\n  \"title\": \"TagList\",\n  \"description\": \"TagList schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tag-list-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: TagList
---
