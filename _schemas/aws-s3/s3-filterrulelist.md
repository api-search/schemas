---
description: A list of containers for the key-value pair that defines the criteria for the filter rule.
layout: schema
name: FilterRuleList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-filterrulelist-schema.json
slug: s3-filterrulelist
source_filename: s3-filterrulelist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FilterRuleList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Name\": {},\n      \"Value\": {}\n    },\n    \"description\": \"Specifies the Amazon S3 object key name to filter on and whether to filter on the suffix or prefix of the key name.\"\n  },\n  \"description\": \"A list of containers for the key-value pair that defines the criteria for the filter rule.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-filterrulelist-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: FilterRuleList
---
