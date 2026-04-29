---
description: TenantInfo schema from Apache Pulsar
layout: schema
name: TenantInfo
properties_list:
- description: ''
  name: adminRoles
  type: array
- description: ''
  name: allowedClusters
  type: array
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-tenant-info-schema.json
slug: apache-pulsar-tenant-info
source_filename: apache-pulsar-tenant-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-tenant-info-schema.json\",\n  \"title\": \"TenantInfo\",\n  \"description\": \"TenantInfo schema from Apache Pulsar\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adminRoles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"allowedClusters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-tenant-info-schema.json
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: TenantInfo
---
