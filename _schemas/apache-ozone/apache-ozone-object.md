---
description: Object schema from Apache Ozone
layout: schema
name: Object
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: lastModified
  type: string
- description: ''
  name: etag
  type: string
- description: ''
  name: size
  type: integer
- description: ''
  name: storageClass
  type: string
- description: ''
  name: owner
  type: object
provider_name: Apache Ozone
provider_slug: apache-ozone
schema_file: json-schema/apache-ozone-object-schema.json
slug: apache-ozone-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-object-schema.json\",\n  \"title\": \"Object\",\n  \"description\": \"Object schema from Apache Ozone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"data/file.csv\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"example\": \"\\\"a1b2c3d4e5f6\\\"\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"example\": 1048576\n    },\n    \"storageClass\": {\n      \"type\": \"string\",\n      \"example\": \"STANDARD\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/Owner\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-object-schema.json
tags:
- Distributed Storage
- Hadoop
- Object Storage
- S3-Compatible
- Apache
- Open Source
title: Object
---
