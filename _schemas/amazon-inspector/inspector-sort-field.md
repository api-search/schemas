---
description: SortField schema
layout: schema
name: SortField
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-sort-field-schema.json
slug: inspector-sort-field
source_filename: inspector-sort-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-sort-field-schema.json\",\n  \"title\": \"SortField\",\n  \"description\": \"SortField schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AWS_ACCOUNT_ID\",\n    \"FINDING_TYPE\",\n    \"SEVERITY\",\n    \"FIRST_OBSERVED_AT\",\n    \"LAST_OBSERVED_AT\",\n    \"FINDING_STATUS\",\n    \"RESOURCE_TYPE\",\n    \"ECR_IMAGE_PUSHED_AT\",\n    \"ECR_IMAGE_REPOSITORY_NAME\",\n    \"ECR_IMAGE_REGISTRY\",\n    \"NETWORK_PROTOCOL\",\n    \"COMPONENT_TYPE\",\n    \"VULNERABILITY_ID\",\n    \"VULNERABILITY_SOURCE\",\n    \"INSPECTOR_SCORE\",\n    \"VENDOR_SEVERITY\",\n    \"EPSS_SCORE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-sort-field-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: SortField
---
