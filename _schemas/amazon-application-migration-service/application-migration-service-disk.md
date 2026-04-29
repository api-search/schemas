---
description: A disk on a source server
layout: schema
name: Disk
properties_list:
- description: Device name
  name: deviceName
  type: string
- description: Disk size in bytes
  name: bytes
  type: integer
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-disk-schema.json
slug: application-migration-service-disk
source_filename: application-migration-service-disk-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-disk-schema.json\",\n  \"title\": \"Disk\",\n  \"description\": \"A disk on a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Device name\"\n    },\n    \"bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Disk size in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-disk-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: Disk
---
