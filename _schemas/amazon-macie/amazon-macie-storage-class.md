---
description: 'The storage class of the S3 object. Possible values are:'
layout: schema
name: StorageClass
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-storage-class-schema.json
slug: amazon-macie-storage-class
source_filename: amazon-macie-storage-class-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-storage-class-schema.json\",\n  \"title\": \"StorageClass\",\n  \"description\": \"The storage class of the S3 object. Possible values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"STANDARD\",\n    \"REDUCED_REDUNDANCY\",\n    \"STANDARD_IA\",\n    \"INTELLIGENT_TIERING\",\n    \"DEEP_ARCHIVE\",\n    \"ONEZONE_IA\",\n    \"GLACIER\",\n    \"GLACIER_IR\",\n    \"OUTPOSTS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-storage-class-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: StorageClass
---
