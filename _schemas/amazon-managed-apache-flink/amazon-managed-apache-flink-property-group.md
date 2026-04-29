---
description: Property key-value pairs passed into an application.
layout: schema
name: PropertyGroup
properties_list:
- description: ''
  name: PropertyGroupId
  type: object
- description: ''
  name: PropertyMap
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-property-group-schema.json
slug: amazon-managed-apache-flink-property-group
source_filename: amazon-managed-apache-flink-property-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-property-group-schema.json\",\n  \"title\": \"PropertyGroup\",\n  \"description\": \"Property key-value pairs passed into an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PropertyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"Describes the key of an application execution property key-value pair.\"\n        }\n      ]\n    },\n    \"PropertyMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyMap\"\n        },\n        {\n          \"description\": \"Describes the value of an application execution property key-value pair.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PropertyGroupId\",\n   \
  \ \"PropertyMap\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-property-group-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: PropertyGroup
---
