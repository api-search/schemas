---
description: Provides information about custom data identifiers that produced a sensitive data finding, and the number of occurrences of the data that each identifier detected.
layout: schema
name: CustomDetections
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-custom-detections-schema.json
slug: amazon-macie-custom-detections
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-custom-detections-schema.json\",\n  \"title\": \"CustomDetections\",\n  \"description\": \"Provides information about custom data identifiers that produced a sensitive data finding, and the number of occurrences of the data that each identifier detected.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/CustomDetection\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-custom-detections-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CustomDetections
---
