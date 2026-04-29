---
description: Bucket schema from Apache Ozone
layout: schema
name: Bucket
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: creationDate
  type: string
- description: ''
  name: storageClass
  type: string
provider_name: Apache Ozone
provider_slug: apache-ozone
schema_file: json-schema/apache-ozone-bucket-schema.json
slug: apache-ozone-bucket
source_filename: apache-ozone-bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-bucket-schema.json\",\n  \"title\": \"Bucket\",\n  \"description\": \"Bucket schema from Apache Ozone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"my-bucket\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    },\n    \"storageClass\": {\n      \"type\": \"string\",\n      \"example\": \"STANDARD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-bucket-schema.json
tags:
- Distributed Storage
- Hadoop
- Object Storage
- S3-Compatible
- Apache
- Open Source
title: Bucket
---
