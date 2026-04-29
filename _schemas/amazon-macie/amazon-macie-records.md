---
description: Specifies the locations of occurrences of sensitive data in an Apache Avro object container or a structured data file.
layout: schema
name: Records
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-records-schema.json
slug: amazon-macie-records
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-records-schema.json\",\n  \"title\": \"Records\",\n  \"description\": \"Specifies the locations of occurrences of sensitive data in an Apache Avro object container or a structured data file.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Record\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-records-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Records
---
