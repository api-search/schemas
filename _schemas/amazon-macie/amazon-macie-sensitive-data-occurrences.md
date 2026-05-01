---
description: Specifies a type of sensitive data reported by a finding and provides occurrences of the specified type of sensitive data.
layout: schema
name: SensitiveDataOccurrences
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-sensitive-data-occurrences-schema.json
slug: amazon-macie-sensitive-data-occurrences
source_filename: amazon-macie-sensitive-data-occurrences-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitive-data-occurrences-schema.json\",\n  \"title\": \"SensitiveDataOccurrences\",\n  \"description\": \"Specifies a type of sensitive data reported by a finding and provides occurrences of the specified type of sensitive data.\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/__listOfDetectedDataDetails\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitive-data-occurrences-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SensitiveDataOccurrences
---
