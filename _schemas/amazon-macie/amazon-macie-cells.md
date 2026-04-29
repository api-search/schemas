---
description: Specifies the location of occurrences of sensitive data in a Microsoft Excel workbook, CSV file, or TSV file.
layout: schema
name: Cells
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-cells-schema.json
slug: amazon-macie-cells
source_filename: amazon-macie-cells-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-cells-schema.json\",\n  \"title\": \"Cells\",\n  \"description\": \"Specifies the location of occurrences of sensitive data in a Microsoft Excel workbook, CSV file, or TSV file.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Cell\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-cells-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Cells
---
