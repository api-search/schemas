---
description: Container for all (if there are any) keys between Prefix and the next occurrence of the string specified by a delimiter.
layout: schema
name: CommonPrefix
properties_list:
- description: Container for the specified common prefix.
  name: Prefix
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-common-prefix-schema.json
slug: amazon-s3-rest-common-prefix
source_filename: amazon-s3-rest-common-prefix-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommonPrefix\",\n  \"type\": \"object\",\n  \"description\": \"Container for all (if there are any) keys between Prefix and the next occurrence of the string specified by a delimiter.\",\n  \"properties\": {\n    \"Prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Container for the specified common prefix.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-common-prefix-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CommonPrefix
---
