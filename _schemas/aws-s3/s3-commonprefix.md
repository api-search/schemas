---
description: Container for all (if there are any) keys between Prefix and the next occurrence of the string specified by a delimiter. CommonPrefixes lists keys that act like subdirectories in the directory specified by Prefix. For example, if the prefix is notes/ and the delimiter is a slash (/) as in notes/summer/july, the common prefix is notes/summer/.
layout: schema
name: CommonPrefix
properties_list:
- description: ''
  name: Prefix
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-commonprefix-schema.json
slug: s3-commonprefix
source_filename: s3-commonprefix-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommonPrefix\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {}\n  },\n  \"description\": \"Container for all (if there are any) keys between Prefix and the next occurrence of the string specified by a delimiter. CommonPrefixes lists keys that act like subdirectories in the directory specified by Prefix. For example, if the prefix is notes/ and the delimiter is a slash (/) as in notes/summer/july, the common prefix is notes/summer/. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-commonprefix-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: CommonPrefix
---
