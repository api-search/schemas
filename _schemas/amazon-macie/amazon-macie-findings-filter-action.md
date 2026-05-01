---
description: 'The action to perform on findings that match the filter criteria. To suppress (automatically archive) findings that match the criteria, set this value to ARCHIVE. Valid values are:'
layout: schema
name: FindingsFilterAction
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-findings-filter-action-schema.json
slug: amazon-macie-findings-filter-action
source_filename: amazon-macie-findings-filter-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-findings-filter-action-schema.json\",\n  \"title\": \"FindingsFilterAction\",\n  \"description\": \"The action to perform on findings that match the filter criteria. To suppress (automatically archive) findings that match the criteria, set this value to ARCHIVE. Valid values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ARCHIVE\",\n    \"NOOP\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-findings-filter-action-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: FindingsFilterAction
---
