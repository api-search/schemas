---
description: Provides information about the tags that are associated with an S3 bucket or object. Each tag consists of a required tag key and an associated tag value.
layout: schema
name: KeyValuePairList
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-key-value-pair-list-schema.json
slug: amazon-macie-key-value-pair-list
source_filename: amazon-macie-key-value-pair-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-key-value-pair-list-schema.json\",\n  \"title\": \"KeyValuePairList\",\n  \"description\": \"Provides information about the tags that are associated with an S3 bucket or object. Each tag consists of a required tag key and an associated tag value.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/KeyValuePair\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-key-value-pair-list-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: KeyValuePairList
---
