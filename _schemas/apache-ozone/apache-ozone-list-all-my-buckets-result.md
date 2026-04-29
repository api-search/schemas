---
description: ListAllMyBucketsResult schema from Apache Ozone
layout: schema
name: ListAllMyBucketsResult
properties_list:
- description: ''
  name: owner
  type: object
- description: ''
  name: buckets
  type: array
provider_name: Apache Ozone
provider_slug: apache-ozone
schema_file: json-schema/apache-ozone-list-all-my-buckets-result-schema.json
slug: apache-ozone-list-all-my-buckets-result
source_filename: apache-ozone-list-all-my-buckets-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-list-all-my-buckets-result-schema.json\",\n  \"title\": \"ListAllMyBucketsResult\",\n  \"description\": \"ListAllMyBucketsResult schema from Apache Ozone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/Owner\"\n    },\n    \"buckets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Bucket\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ozone/refs/heads/main/json-schema/apache-ozone-list-all-my-buckets-result-schema.json
tags:
- Distributed Storage
- Hadoop
- Object Storage
- S3-Compatible
- Apache
- Open Source
title: ListAllMyBucketsResult
---
