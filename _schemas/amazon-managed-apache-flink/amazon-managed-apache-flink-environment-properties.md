---
description: Describes execution properties for a Flink-based Kinesis Data Analytics application.
layout: schema
name: EnvironmentProperties
properties_list:
- description: ''
  name: PropertyGroups
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-environment-properties-schema.json
slug: amazon-managed-apache-flink-environment-properties
source_filename: amazon-managed-apache-flink-environment-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-environment-properties-schema.json\",\n  \"title\": \"EnvironmentProperties\",\n  \"description\": \"Describes execution properties for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PropertyGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyGroups\"\n        },\n        {\n          \"description\": \"Describes the execution property groups.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PropertyGroups\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-environment-properties-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: EnvironmentProperties
---
