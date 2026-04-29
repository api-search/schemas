---
description: Owner schema from Apache Ozone
layout: schema
name: Owner
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: displayName
  type: string
provider_name: Apache Ozone
provider_slug: apache-ozone
schema_file: json-schema/apache-ozone-owner-schema.json
slug: apache-ozone-owner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-owner-schema.json\",\n  \"title\": \"Owner\",\n  \"description\": \"Owner schema from Apache Ozone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ozone-user-001\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"ozone-admin\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-owner-schema.json
tags:
- Distributed Storage
- Hadoop
- Object Storage
- S3-Compatible
- Apache
- Open Source
title: Owner
---
