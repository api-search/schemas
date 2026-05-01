---
description: 'Indicates the current status of an allow list. Depending on the type of criteria that the list specifies, possible values are:'
layout: schema
name: AllowListStatusCode
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-allow-list-status-code-schema.json
slug: amazon-macie-allow-list-status-code
source_filename: amazon-macie-allow-list-status-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-status-code-schema.json\",\n  \"title\": \"AllowListStatusCode\",\n  \"description\": \"Indicates the current status of an allow list. Depending on the type of criteria that the list specifies, possible values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"OK\",\n    \"S3_OBJECT_NOT_FOUND\",\n    \"S3_USER_ACCESS_DENIED\",\n    \"S3_OBJECT_ACCESS_DENIED\",\n    \"S3_THROTTLED\",\n    \"S3_OBJECT_OVERSIZE\",\n    \"S3_OBJECT_EMPTY\",\n    \"UNKNOWN_ERROR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-status-code-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AllowListStatusCode
---
