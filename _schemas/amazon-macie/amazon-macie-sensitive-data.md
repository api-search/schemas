---
description: Provides information about the category and number of occurrences of sensitive data that produced a finding.
layout: schema
name: SensitiveData
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-sensitive-data-schema.json
slug: amazon-macie-sensitive-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitive-data-schema.json\",\n  \"title\": \"SensitiveData\",\n  \"description\": \"Provides information about the category and number of occurrences of sensitive data that produced a finding.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/SensitiveDataItem\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitive-data-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SensitiveData
---
